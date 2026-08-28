# BatchSendShipments200ResponseSummary

Aggregate counts for the batch.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**total** | **int** | Number of unique shipments requested. | 
**sent** | **int** | How many were successfully booked. | 
**failed** | **int** | How many the carrier or Zippendo rejected. | 
**skipped** | **int** | How many the batch ran out of time to attempt. Submit these again. | 

## Example

```python
from zippendo.models.batch_send_shipments200_response_summary import BatchSendShipments200ResponseSummary

# TODO update the JSON string below
json = "{}"
# create an instance of BatchSendShipments200ResponseSummary from a JSON string
batch_send_shipments200_response_summary_instance = BatchSendShipments200ResponseSummary.from_json(json)
# print the JSON string representation of the object
print(BatchSendShipments200ResponseSummary.to_json())

# convert the object into a dict
batch_send_shipments200_response_summary_dict = batch_send_shipments200_response_summary_instance.to_dict()
# create an instance of BatchSendShipments200ResponseSummary from a dict
batch_send_shipments200_response_summary_from_dict = BatchSendShipments200ResponseSummary.from_dict(batch_send_shipments200_response_summary_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


