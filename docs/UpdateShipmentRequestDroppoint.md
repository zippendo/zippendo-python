# UpdateShipmentRequestDroppoint

Display details of the selected service point, stored alongside `servicePointId`. Used when applying a service-point shipping rule (whose parameters otherwise replace the stored droppoint).

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | Identifier of the selected service point. | 
**name** | **str** | Display name of the service point. | 
**address** | **str** | Formatted address of the service point. | 
**coordinates** | [**List[ListShippingRules200ResponseDataInnerAdditionalParametersValueAnyOfCoordinatesInner]**](ListShippingRules200ResponseDataInnerAdditionalParametersValueAnyOfCoordinatesInner.md) | Latitude/longitude of the service point. | [optional] 

## Example

```python
from zippendo.models.update_shipment_request_droppoint import UpdateShipmentRequestDroppoint

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateShipmentRequestDroppoint from a JSON string
update_shipment_request_droppoint_instance = UpdateShipmentRequestDroppoint.from_json(json)
# print the JSON string representation of the object
print(UpdateShipmentRequestDroppoint.to_json())

# convert the object into a dict
update_shipment_request_droppoint_dict = update_shipment_request_droppoint_instance.to_dict()
# create an instance of UpdateShipmentRequestDroppoint from a dict
update_shipment_request_droppoint_from_dict = UpdateShipmentRequestDroppoint.from_dict(update_shipment_request_droppoint_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


