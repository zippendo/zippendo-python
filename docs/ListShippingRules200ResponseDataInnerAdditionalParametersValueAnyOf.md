# ListShippingRules200ResponseDataInnerAdditionalParametersValueAnyOf


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | Identifier of the selected service point. | 
**name** | **str** | Display name of the service point. | 
**address** | **str** | Formatted address of the service point. | 
**coordinates** | [**List[ListShippingRules200ResponseDataInnerAdditionalParametersValueAnyOfCoordinatesInner]**](ListShippingRules200ResponseDataInnerAdditionalParametersValueAnyOfCoordinatesInner.md) | Latitude/longitude of the service point. | [optional] 

## Example

```python
from zippendo.models.list_shipping_rules200_response_data_inner_additional_parameters_value_any_of import ListShippingRules200ResponseDataInnerAdditionalParametersValueAnyOf

# TODO update the JSON string below
json = "{}"
# create an instance of ListShippingRules200ResponseDataInnerAdditionalParametersValueAnyOf from a JSON string
list_shipping_rules200_response_data_inner_additional_parameters_value_any_of_instance = ListShippingRules200ResponseDataInnerAdditionalParametersValueAnyOf.from_json(json)
# print the JSON string representation of the object
print(ListShippingRules200ResponseDataInnerAdditionalParametersValueAnyOf.to_json())

# convert the object into a dict
list_shipping_rules200_response_data_inner_additional_parameters_value_any_of_dict = list_shipping_rules200_response_data_inner_additional_parameters_value_any_of_instance.to_dict()
# create an instance of ListShippingRules200ResponseDataInnerAdditionalParametersValueAnyOf from a dict
list_shipping_rules200_response_data_inner_additional_parameters_value_any_of_from_dict = ListShippingRules200ResponseDataInnerAdditionalParametersValueAnyOf.from_dict(list_shipping_rules200_response_data_inner_additional_parameters_value_any_of_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


