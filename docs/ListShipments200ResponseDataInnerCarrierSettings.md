# ListShipments200ResponseDataInnerCarrierSettings


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**carrier_id** | **str** | Identifier of the carrier to use. | 
**product_id** | **str** | Identifier of the carrier product/service. | 
**services** | **List[str]** | Additional service codes requested from the carrier. | 
**additional_parameters** | [**Dict[str, ListShipments200ResponseDataInnerCarrierSettingsAdditionalParametersValue]**](ListShipments200ResponseDataInnerCarrierSettingsAdditionalParametersValue.md) | Carrier-specific extra parameters as key/value pairs. | 

## Example

```python
from zippendo.models.list_shipments200_response_data_inner_carrier_settings import ListShipments200ResponseDataInnerCarrierSettings

# TODO update the JSON string below
json = "{}"
# create an instance of ListShipments200ResponseDataInnerCarrierSettings from a JSON string
list_shipments200_response_data_inner_carrier_settings_instance = ListShipments200ResponseDataInnerCarrierSettings.from_json(json)
# print the JSON string representation of the object
print(ListShipments200ResponseDataInnerCarrierSettings.to_json())

# convert the object into a dict
list_shipments200_response_data_inner_carrier_settings_dict = list_shipments200_response_data_inner_carrier_settings_instance.to_dict()
# create an instance of ListShipments200ResponseDataInnerCarrierSettings from a dict
list_shipments200_response_data_inner_carrier_settings_from_dict = ListShipments200ResponseDataInnerCarrierSettings.from_dict(list_shipments200_response_data_inner_carrier_settings_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


