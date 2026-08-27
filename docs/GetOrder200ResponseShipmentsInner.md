# GetOrder200ResponseShipmentsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | Unique shipment identifier. | 
**reference** | **str** | Customer-facing shipment reference. | 
**status** | **str** | Lifecycle status of the shipment. | 
**type** | **str** | Direction of the shipment relative to the organization. | 
**tracking** | [**CreateShipment201ResponseTracking**](CreateShipment201ResponseTracking.md) |  | [optional] 
**carrier_settings** | [**ListShipments200ResponseDataInnerCarrierSettings**](ListShipments200ResponseDataInnerCarrierSettings.md) |  | 
**service_point_id** | **str** | Selected carrier service point identifier. | [optional] 
**created_at** | **str** | Timestamp when the shipment was created. | 
**updated_at** | **str** | Timestamp when the shipment was last updated. | 
**shipping_rule_id** | **str** | ID of the shipping rule used for this shipment. | [optional] 
**documents** | [**List[CreateShipment201ResponseDocumentsInner]**](CreateShipment201ResponseDocumentsInner.md) | Documents (labels, customs forms) for this shipment. | [optional] 

## Example

```python
from zippendo.models.get_order200_response_shipments_inner import GetOrder200ResponseShipmentsInner

# TODO update the JSON string below
json = "{}"
# create an instance of GetOrder200ResponseShipmentsInner from a JSON string
get_order200_response_shipments_inner_instance = GetOrder200ResponseShipmentsInner.from_json(json)
# print the JSON string representation of the object
print(GetOrder200ResponseShipmentsInner.to_json())

# convert the object into a dict
get_order200_response_shipments_inner_dict = get_order200_response_shipments_inner_instance.to_dict()
# create an instance of GetOrder200ResponseShipmentsInner from a dict
get_order200_response_shipments_inner_from_dict = GetOrder200ResponseShipmentsInner.from_dict(get_order200_response_shipments_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


