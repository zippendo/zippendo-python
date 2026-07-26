# ListShipments200ResponseDataInnerCarrierSettingsAdditionalParametersValueAnyOf


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | Identifier of the selected service point. | 
**name** | **str** | Display name of the service point. | 
**address** | **str** | Formatted address of the service point. | 
**coordinates** | [**List[CreateShippingRuleRequestAdditionalParametersAnyOfValueAnyOfCoordinatesInner]**](CreateShippingRuleRequestAdditionalParametersAnyOfValueAnyOfCoordinatesInner.md) | Latitude/longitude of the service point. | [optional] 

## Example

```python
from zippendo.models.list_shipments200_response_data_inner_carrier_settings_additional_parameters_value_any_of import ListShipments200ResponseDataInnerCarrierSettingsAdditionalParametersValueAnyOf

# TODO update the JSON string below
json = "{}"
# create an instance of ListShipments200ResponseDataInnerCarrierSettingsAdditionalParametersValueAnyOf from a JSON string
list_shipments200_response_data_inner_carrier_settings_additional_parameters_value_any_of_instance = ListShipments200ResponseDataInnerCarrierSettingsAdditionalParametersValueAnyOf.from_json(json)
# print the JSON string representation of the object
print(ListShipments200ResponseDataInnerCarrierSettingsAdditionalParametersValueAnyOf.to_json())

# convert the object into a dict
list_shipments200_response_data_inner_carrier_settings_additional_parameters_value_any_of_dict = list_shipments200_response_data_inner_carrier_settings_additional_parameters_value_any_of_instance.to_dict()
# create an instance of ListShipments200ResponseDataInnerCarrierSettingsAdditionalParametersValueAnyOf from a dict
list_shipments200_response_data_inner_carrier_settings_additional_parameters_value_any_of_from_dict = ListShipments200ResponseDataInnerCarrierSettingsAdditionalParametersValueAnyOf.from_dict(list_shipments200_response_data_inner_carrier_settings_additional_parameters_value_any_of_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


