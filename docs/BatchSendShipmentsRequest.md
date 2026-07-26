# BatchSendShipmentsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**shipment_ids** | **List[str]** | IDs of the shipments to book. Each must be in &#x60;pending&#x60; or &#x60;error&#x60; status; duplicates are ignored. Max 100 per request. | 

## Example

```python
from zippendo.models.batch_send_shipments_request import BatchSendShipmentsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of BatchSendShipmentsRequest from a JSON string
batch_send_shipments_request_instance = BatchSendShipmentsRequest.from_json(json)
# print the JSON string representation of the object
print(BatchSendShipmentsRequest.to_json())

# convert the object into a dict
batch_send_shipments_request_dict = batch_send_shipments_request_instance.to_dict()
# create an instance of BatchSendShipmentsRequest from a dict
batch_send_shipments_request_from_dict = BatchSendShipmentsRequest.from_dict(batch_send_shipments_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


