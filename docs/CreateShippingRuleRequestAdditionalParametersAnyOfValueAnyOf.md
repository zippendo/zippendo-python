# CreateShippingRuleRequestAdditionalParametersAnyOfValueAnyOf


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | Identifier of the selected service point. | 
**name** | **str** | Display name of the service point. | 
**address** | **str** | Formatted address of the service point. | 
**coordinates** | [**List[CreateShippingRuleRequestAdditionalParametersAnyOfValueAnyOfCoordinatesInner]**](CreateShippingRuleRequestAdditionalParametersAnyOfValueAnyOfCoordinatesInner.md) | Latitude/longitude of the service point. | [optional] 

## Example

```python
from zippendo.models.create_shipping_rule_request_additional_parameters_any_of_value_any_of import CreateShippingRuleRequestAdditionalParametersAnyOfValueAnyOf

# TODO update the JSON string below
json = "{}"
# create an instance of CreateShippingRuleRequestAdditionalParametersAnyOfValueAnyOf from a JSON string
create_shipping_rule_request_additional_parameters_any_of_value_any_of_instance = CreateShippingRuleRequestAdditionalParametersAnyOfValueAnyOf.from_json(json)
# print the JSON string representation of the object
print(CreateShippingRuleRequestAdditionalParametersAnyOfValueAnyOf.to_json())

# convert the object into a dict
create_shipping_rule_request_additional_parameters_any_of_value_any_of_dict = create_shipping_rule_request_additional_parameters_any_of_value_any_of_instance.to_dict()
# create an instance of CreateShippingRuleRequestAdditionalParametersAnyOfValueAnyOf from a dict
create_shipping_rule_request_additional_parameters_any_of_value_any_of_from_dict = CreateShippingRuleRequestAdditionalParametersAnyOfValueAnyOf.from_dict(create_shipping_rule_request_additional_parameters_any_of_value_any_of_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


