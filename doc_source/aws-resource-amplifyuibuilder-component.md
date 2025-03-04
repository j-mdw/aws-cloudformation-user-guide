# AWS::AmplifyUIBuilder::Component<a name="aws-resource-amplifyuibuilder-component"></a>

The AWS::AmplifyUIBuilder::Component resource specifies a component within an Amplify app\. A component is a user interface \(UI\) element that you can customize\. Use `ComponentChild` to configure an instance of a `Component`\. A `ComponentChild` instance inherits the configuration of the main `Component`\.

## Syntax<a name="aws-resource-amplifyuibuilder-component-syntax"></a>

To declare this entity in your AWS CloudFormation template, use the following syntax:

### JSON<a name="aws-resource-amplifyuibuilder-component-syntax.json"></a>

```
{
  "Type" : "AWS::AmplifyUIBuilder::Component",
  "Properties" : {
      "[BindingProperties](#cfn-amplifyuibuilder-component-bindingproperties)" : {Key : Value, ...},
      "[Children](#cfn-amplifyuibuilder-component-children)" : [ ComponentChild, ... ],
      "[CollectionProperties](#cfn-amplifyuibuilder-component-collectionproperties)" : {Key : Value, ...},
      "[ComponentType](#cfn-amplifyuibuilder-component-componenttype)" : String,
      "[Name](#cfn-amplifyuibuilder-component-name)" : String,
      "[Overrides](#cfn-amplifyuibuilder-component-overrides)" : {Key : Value, ...},
      "[Properties](#cfn-amplifyuibuilder-component-properties)" : {Key : Value, ...},
      "[SourceId](#cfn-amplifyuibuilder-component-sourceid)" : String,
      "[Tags](#cfn-amplifyuibuilder-component-tags)" : {Key : Value, ...},
      "[Variants](#cfn-amplifyuibuilder-component-variants)" : [ ComponentVariant, ... ]
    }
}
```

### YAML<a name="aws-resource-amplifyuibuilder-component-syntax.yaml"></a>

```
Type: AWS::AmplifyUIBuilder::Component
Properties: 
  [BindingProperties](#cfn-amplifyuibuilder-component-bindingproperties): 
    Key : Value
  [Children](#cfn-amplifyuibuilder-component-children): 
    - ComponentChild
  [CollectionProperties](#cfn-amplifyuibuilder-component-collectionproperties): 
    Key : Value
  [ComponentType](#cfn-amplifyuibuilder-component-componenttype): String
  [Name](#cfn-amplifyuibuilder-component-name): String
  [Overrides](#cfn-amplifyuibuilder-component-overrides): 
    Key : Value
  [Properties](#cfn-amplifyuibuilder-component-properties): 
    Key : Value
  [SourceId](#cfn-amplifyuibuilder-component-sourceid): String
  [Tags](#cfn-amplifyuibuilder-component-tags): 
    Key : Value
  [Variants](#cfn-amplifyuibuilder-component-variants): 
    - ComponentVariant
```

## Properties<a name="aws-resource-amplifyuibuilder-component-properties"></a>

`BindingProperties`  <a name="cfn-amplifyuibuilder-component-bindingproperties"></a>
The information to connect a component's properties to data at runtime\. You can't specify `tags` as a valid property for `bindingProperties`\.  
  
*Required*: No  
*Type*: Map of [ComponentBindingPropertiesValue](aws-properties-amplifyuibuilder-component-componentbindingpropertiesvalue.md)  
*Update requires*: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

`Children`  <a name="cfn-amplifyuibuilder-component-children"></a>
A list of the component's `ComponentChild` instances\.  
*Required*: No  
*Type*: List of [ComponentChild](aws-properties-amplifyuibuilder-component-componentchild.md)  
*Update requires*: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

`CollectionProperties`  <a name="cfn-amplifyuibuilder-component-collectionproperties"></a>
The data binding configuration for the component's properties\. Use this for a collection component\. You can't specify `tags` as a valid property for `collectionProperties`\.  
*Required*: No  
*Type*: Map of [ComponentDataConfiguration](aws-properties-amplifyuibuilder-component-componentdataconfiguration.md)  
*Update requires*: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

`ComponentType`  <a name="cfn-amplifyuibuilder-component-componenttype"></a>
The type of the component\. This can be an Amplify custom UI component or another custom component\.  
*Required*: No  
*Type*: String  
*Update requires*: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

`Name`  <a name="cfn-amplifyuibuilder-component-name"></a>
The name of the component\.  
*Required*: No  
*Type*: String  
*Update requires*: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

`Overrides`  <a name="cfn-amplifyuibuilder-component-overrides"></a>
Describes the component's properties that can be overriden in a customized instance of the component\. You can't specify `tags` as a valid property for `overrides`\.  
*Required*: No  
*Type*: Map of [ComponentOverridesValue](aws-properties-amplifyuibuilder-component-componentoverridesvalue.md)  
*Update requires*: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

`Properties`  <a name="cfn-amplifyuibuilder-component-properties"></a>
Describes the component's properties\. You can't specify `tags` as a valid property for `properties`\.  
*Required*: No  
*Type*: Map of [ComponentProperty](aws-properties-amplifyuibuilder-component-componentproperty.md)  
*Update requires*: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

`SourceId`  <a name="cfn-amplifyuibuilder-component-sourceid"></a>
The unique ID of the component in its original source system, such as Figma\.  
*Required*: No  
*Type*: String  
*Update requires*: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

`Tags`  <a name="cfn-amplifyuibuilder-component-tags"></a>
One or more key\-value pairs to use when tagging the component\.  
*Required*: No  
*Type*: Map of String  
*Update requires*: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement)

`Variants`  <a name="cfn-amplifyuibuilder-component-variants"></a>
A list of the component's variants\. A variant is a unique style configuration of a main component\.  
*Required*: No  
*Type*: List of [ComponentVariant](aws-properties-amplifyuibuilder-component-componentvariant.md)  
*Update requires*: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

## Return values<a name="aws-resource-amplifyuibuilder-component-return-values"></a>

### Ref<a name="aws-resource-amplifyuibuilder-component-return-values-ref"></a>

### Fn::GetAtt<a name="aws-resource-amplifyuibuilder-component-return-values-fn--getatt"></a>

The `Fn::GetAtt` intrinsic function returns a value for a specified attribute of this type\. The following are the available attributes and sample return values\.

For more information about using the `Fn::GetAtt` intrinsic function, see [Fn::GetAtt](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/intrinsic-function-reference-getatt.html)\.

#### <a name="aws-resource-amplifyuibuilder-component-return-values-fn--getatt-fn--getatt"></a>

`AppId`  <a name="AppId-fn::getatt"></a>
The unique ID for the Amplify app\.

`CreatedAt`  <a name="CreatedAt-fn::getatt"></a>
The time that the component was created\.

`EnvironmentName`  <a name="EnvironmentName-fn::getatt"></a>
The name of the backend environment that is a part of the Amplify app\.

`Id`  <a name="Id-fn::getatt"></a>
The unique ID of the component\.

`ModifiedAt`  <a name="ModifiedAt-fn::getatt"></a>
The time that the component was modified\.