# CreateShipmentRequestDroppoint

Display details of the selected service point, stored alongside `servicePointId`. Used with a service-point shipping rule.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | Identifier of the selected service point. | 
**name** | **str** | Display name of the service point. | 
**address** | **str** | Formatted address of the service point. | 
**coordinates** | [**List[ListShippingRules200ResponseDataInnerAdditionalParametersValueAnyOfCoordinatesInner]**](ListShippingRules200ResponseDataInnerAdditionalParametersValueAnyOfCoordinatesInner.md) | Latitude/longitude of the service point. | [optional] 

## Example

```python
from zippendo.models.create_shipment_request_droppoint import CreateShipmentRequestDroppoint

# TODO update the JSON string below
json = "{}"
# create an instance of CreateShipmentRequestDroppoint from a JSON string
create_shipment_request_droppoint_instance = CreateShipmentRequestDroppoint.from_json(json)
# print the JSON string representation of the object
print(CreateShipmentRequestDroppoint.to_json())

# convert the object into a dict
create_shipment_request_droppoint_dict = create_shipment_request_droppoint_instance.to_dict()
# create an instance of CreateShipmentRequestDroppoint from a dict
create_shipment_request_droppoint_from_dict = CreateShipmentRequestDroppoint.from_dict(create_shipment_request_droppoint_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


