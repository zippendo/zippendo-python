# CreateShipmentRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**reference** | **str** | Customer-facing shipment reference. | [optional] 
**address_id** | **str** | Sender address identifier. | [optional] 
**service_point_id** | **str** | Selected carrier service point identifier. | [optional] 
**parties** | [**List[CreateShipmentRequestPartiesInner]**](CreateShipmentRequestPartiesInner.md) | Parties involved in the shipment. Optional when orderId is provided. | [optional] 
**type** | **str** | Direction of the shipment relative to the organization. | 
**carrier_settings** | [**CreateShipmentRequestCarrierSettings**](CreateShipmentRequestCarrierSettings.md) |  | 
**parcels** | [**List[CreateShipmentRequestParcelsInner]**](CreateShipmentRequestParcelsInner.md) | Parcels to include. Optional when orderId is provided. | [optional] 
**pickup_details** | [**CreateShipmentRequestPickupDetails**](CreateShipmentRequestPickupDetails.md) |  | [optional] 
**term_of_trade** | **str** | Incoterm governing the shipment. | [optional] [default to 'DAP']
**status** | **str** | Lifecycle status of the shipment. | [optional] [default to 'pending']
**order_id** | **str** | Order to derive parties and parcels from. | [optional] 
**label_printer_id** | **str** | Printer to assign for labels. | [optional] 
**document_printer_id** | **str** | Printer to assign for documents. | [optional] 

## Example

```python
from zippendo.models.create_shipment_request import CreateShipmentRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateShipmentRequest from a JSON string
create_shipment_request_instance = CreateShipmentRequest.from_json(json)
# print the JSON string representation of the object
print(CreateShipmentRequest.to_json())

# convert the object into a dict
create_shipment_request_dict = create_shipment_request_instance.to_dict()
# create an instance of CreateShipmentRequest from a dict
create_shipment_request_from_dict = CreateShipmentRequest.from_dict(create_shipment_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


