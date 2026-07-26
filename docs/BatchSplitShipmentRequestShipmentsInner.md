# BatchSplitShipmentRequestShipmentsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**reference** | **str** | Reference for this new shipment. Defaults to original reference with a suffix. | [optional] 
**order_lines** | [**List[BatchSplitShipmentRequestShipmentsInnerOrderLinesInner]**](BatchSplitShipmentRequestShipmentsInnerOrderLinesInner.md) | Order lines and quantities to move into this new shipment. | 

## Example

```python
from zippendo.models.batch_split_shipment_request_shipments_inner import BatchSplitShipmentRequestShipmentsInner

# TODO update the JSON string below
json = "{}"
# create an instance of BatchSplitShipmentRequestShipmentsInner from a JSON string
batch_split_shipment_request_shipments_inner_instance = BatchSplitShipmentRequestShipmentsInner.from_json(json)
# print the JSON string representation of the object
print(BatchSplitShipmentRequestShipmentsInner.to_json())

# convert the object into a dict
batch_split_shipment_request_shipments_inner_dict = batch_split_shipment_request_shipments_inner_instance.to_dict()
# create an instance of BatchSplitShipmentRequestShipmentsInner from a dict
batch_split_shipment_request_shipments_inner_from_dict = BatchSplitShipmentRequestShipmentsInner.from_dict(batch_split_shipment_request_shipments_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


