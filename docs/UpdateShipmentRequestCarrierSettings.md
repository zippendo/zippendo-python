# UpdateShipmentRequestCarrierSettings


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**carrier_id** | **str** | Identifier of the carrier to use. | 
**product_id** | **str** | Identifier of the carrier product/service. | 
**services** | **List[str]** | Additional service codes requested from the carrier. | 
**additional_parameters** | [**Dict[str, CreateShippingRuleRequestAdditionalParametersValue]**](CreateShippingRuleRequestAdditionalParametersValue.md) | Carrier-specific extra parameters as key/value pairs. | 

## Example

```python
from zippendo.models.update_shipment_request_carrier_settings import UpdateShipmentRequestCarrierSettings

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateShipmentRequestCarrierSettings from a JSON string
update_shipment_request_carrier_settings_instance = UpdateShipmentRequestCarrierSettings.from_json(json)
# print the JSON string representation of the object
print(UpdateShipmentRequestCarrierSettings.to_json())

# convert the object into a dict
update_shipment_request_carrier_settings_dict = update_shipment_request_carrier_settings_instance.to_dict()
# create an instance of UpdateShipmentRequestCarrierSettings from a dict
update_shipment_request_carrier_settings_from_dict = UpdateShipmentRequestCarrierSettings.from_dict(update_shipment_request_carrier_settings_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


