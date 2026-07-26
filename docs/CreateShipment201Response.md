# CreateShipment201Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | Unique shipment identifier. | 
**reference** | **str** | Customer-facing shipment reference. | 
**address_id** | **str** | Sender address identifier. | [optional] 
**service_point_id** | **str** | Selected carrier service point identifier. | [optional] 
**parties** | [**List[CreateShipment201ResponsePartiesInner]**](CreateShipment201ResponsePartiesInner.md) | Parties involved in the shipment (sender, receiver, etc.). | 
**type** | **str** | Direction of the shipment relative to the organization. | 
**carrier_settings** | [**ListShipments200ResponseDataInnerCarrierSettings**](ListShipments200ResponseDataInnerCarrierSettings.md) |  | 
**parcels** | [**List[CreateShipment201ResponseParcelsInner]**](CreateShipment201ResponseParcelsInner.md) | Parcels included in the shipment. | 
**pickup_details** | [**CreateShipment201ResponsePickupDetails**](CreateShipment201ResponsePickupDetails.md) |  | [optional] 
**term_of_trade** | **str** | Incoterm governing the shipment. | [default to 'DAP']
**documents** | [**List[CreateShipment201ResponseDocumentsInner]**](CreateShipment201ResponseDocumentsInner.md) | Documents generated for the shipment (labels, invoices). | [optional] 
**errors** | [**List[CreateShipment201ResponseErrorsInner]**](CreateShipment201ResponseErrorsInner.md) | Carrier errors recorded for the shipment. | [default to []]
**tracking** | [**CreateShipment201ResponseTracking**](CreateShipment201ResponseTracking.md) |  | [optional] 
**status** | **str** | Lifecycle status of the shipment. | 
**org_id** | **str** | Owning organization identifier. | 
**order_id** | **str** | Associated order identifier. | [optional] 
**shipping_rule_id** | **str** | Applied shipping rule identifier. | [optional] 
**shipping_rule** | [**CreateShipment201ResponseShippingRule**](CreateShipment201ResponseShippingRule.md) |  | [optional] 
**label_printer_id** | **str** | Printer assigned for labels on this shipment. | [optional] 
**document_printer_id** | **str** | Printer assigned for documents on this shipment. | [optional] 
**logs** | [**List[CreateShipment201ResponseLogsInner]**](CreateShipment201ResponseLogsInner.md) | Request/response logs captured during carrier interactions. | [default to []]
**activities** | [**List[CreateShipment201ResponseActivitiesInner]**](CreateShipment201ResponseActivitiesInner.md) | Chronological activity history of the shipment. | [default to []]
**created_at** | **str** | Timestamp when the shipment was created. | 
**updated_at** | **str** | Timestamp when the shipment was last updated. | 

## Example

```python
from zippendo.models.create_shipment201_response import CreateShipment201Response

# TODO update the JSON string below
json = "{}"
# create an instance of CreateShipment201Response from a JSON string
create_shipment201_response_instance = CreateShipment201Response.from_json(json)
# print the JSON string representation of the object
print(CreateShipment201Response.to_json())

# convert the object into a dict
create_shipment201_response_dict = create_shipment201_response_instance.to_dict()
# create an instance of CreateShipment201Response from a dict
create_shipment201_response_from_dict = CreateShipment201Response.from_dict(create_shipment201_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


