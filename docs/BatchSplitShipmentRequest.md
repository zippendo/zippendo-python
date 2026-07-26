# BatchSplitShipmentRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**parcel_id** | **str** | Parcel whose order lines are split across new shipments. | 
**shipments** | [**List[BatchSplitShipmentRequestShipmentsInner]**](BatchSplitShipmentRequestShipmentsInner.md) | New shipments to create from the split parcel. | 
**carrier_id** | **str** | Carrier for all new shipments. Copied from the original if omitted. | [optional] 
**product_id** | **str** | Carrier product for all new shipments. Copied from the original if omitted. | [optional] 
**services** | **List[str]** | Service codes for all new shipments. Copied from the original if omitted. | [optional] 
**additional_parameters** | **Dict[str, object]** | Carrier-specific parameters for all new shipments. | [optional] 

## Example

```python
from zippendo.models.batch_split_shipment_request import BatchSplitShipmentRequest

# TODO update the JSON string below
json = "{}"
# create an instance of BatchSplitShipmentRequest from a JSON string
batch_split_shipment_request_instance = BatchSplitShipmentRequest.from_json(json)
# print the JSON string representation of the object
print(BatchSplitShipmentRequest.to_json())

# convert the object into a dict
batch_split_shipment_request_dict = batch_split_shipment_request_instance.to_dict()
# create an instance of BatchSplitShipmentRequest from a dict
batch_split_shipment_request_from_dict = BatchSplitShipmentRequest.from_dict(batch_split_shipment_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


