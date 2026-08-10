# CreateShipmentRequestCarrierSettings


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**carrier_id** | **str** | Identifier of the carrier to use. | 
**product_id** | **str** | Identifier of the carrier product/service. | 
**services** | **List[str]** | Additional service codes requested from the carrier. | 
**additional_parameters** | [**Dict[str, CreateShippingRuleRequestAdditionalParametersValue]**](CreateShippingRuleRequestAdditionalParametersValue.md) | Carrier-specific extra parameters as key/value pairs. | 

## Example

```python
from zippendo.models.create_shipment_request_carrier_settings import CreateShipmentRequestCarrierSettings

# TODO update the JSON string below
json = "{}"
# create an instance of CreateShipmentRequestCarrierSettings from a JSON string
create_shipment_request_carrier_settings_instance = CreateShipmentRequestCarrierSettings.from_json(json)
# print the JSON string representation of the object
print(CreateShipmentRequestCarrierSettings.to_json())

# convert the object into a dict
create_shipment_request_carrier_settings_dict = create_shipment_request_carrier_settings_instance.to_dict()
# create an instance of CreateShipmentRequestCarrierSettings from a dict
create_shipment_request_carrier_settings_from_dict = CreateShipmentRequestCarrierSettings.from_dict(create_shipment_request_carrier_settings_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


