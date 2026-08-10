# CreateShippingRuleRequestAdditionalParametersValue


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | Identifier of the selected service point. | 
**name** | **str** | Display name of the service point. | 
**address** | **str** | Formatted address of the service point. | 
**coordinates** | [**List[ListShippingRules200ResponseDataInnerAdditionalParametersValueAnyOfCoordinatesInner]**](ListShippingRules200ResponseDataInnerAdditionalParametersValueAnyOfCoordinatesInner.md) | Latitude/longitude of the service point. | [optional] 

## Example

```python
from zippendo.models.create_shipping_rule_request_additional_parameters_value import CreateShippingRuleRequestAdditionalParametersValue

# TODO update the JSON string below
json = "{}"
# create an instance of CreateShippingRuleRequestAdditionalParametersValue from a JSON string
create_shipping_rule_request_additional_parameters_value_instance = CreateShippingRuleRequestAdditionalParametersValue.from_json(json)
# print the JSON string representation of the object
print(CreateShippingRuleRequestAdditionalParametersValue.to_json())

# convert the object into a dict
create_shipping_rule_request_additional_parameters_value_dict = create_shipping_rule_request_additional_parameters_value_instance.to_dict()
# create an instance of CreateShippingRuleRequestAdditionalParametersValue from a dict
create_shipping_rule_request_additional_parameters_value_from_dict = CreateShippingRuleRequestAdditionalParametersValue.from_dict(create_shipping_rule_request_additional_parameters_value_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


