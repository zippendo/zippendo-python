# BatchSendShipments200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**results** | [**List[BatchSendShipments200ResponseResultsInner]**](BatchSendShipments200ResponseResultsInner.md) | Per-shipment outcome (one entry per unique requested shipment id). | 
**summary** | [**BatchSendShipments200ResponseSummary**](BatchSendShipments200ResponseSummary.md) |  | 

## Example

```python
from zippendo.models.batch_send_shipments200_response import BatchSendShipments200Response

# TODO update the JSON string below
json = "{}"
# create an instance of BatchSendShipments200Response from a JSON string
batch_send_shipments200_response_instance = BatchSendShipments200Response.from_json(json)
# print the JSON string representation of the object
print(BatchSendShipments200Response.to_json())

# convert the object into a dict
batch_send_shipments200_response_dict = batch_send_shipments200_response_instance.to_dict()
# create an instance of BatchSendShipments200Response from a dict
batch_send_shipments200_response_from_dict = BatchSendShipments200Response.from_dict(batch_send_shipments200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


