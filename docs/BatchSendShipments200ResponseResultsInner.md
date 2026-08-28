# BatchSendShipments200ResponseResultsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**shipment_id** | **str** | The shipment this result refers to. | 
**status** | **str** | &#x60;sent&#x60; when the carrier booked it, &#x60;failed&#x60; when the carrier or Zippendo rejected it, and &#x60;skipped&#x60; when the batch ran out of time before reaching it. A &#x60;skipped&#x60; shipment was never sent to the carrier and is safe to submit again. | 
**code** | **str** | Canonical machine-readable error code, present when &#x60;status&#x60; is &#x60;failed&#x60; or &#x60;skipped&#x60;. | [optional] 
**message** | **str** | Human-readable detail, present when &#x60;status&#x60; is &#x60;failed&#x60; or &#x60;skipped&#x60;. | [optional] 
**errors** | [**List[SendShipment422ResponseErrorsInner]**](SendShipment422ResponseErrorsInner.md) | Carrier-specific errors, present when the carrier rejected the booking. | [optional] 

## Example

```python
from zippendo.models.batch_send_shipments200_response_results_inner import BatchSendShipments200ResponseResultsInner

# TODO update the JSON string below
json = "{}"
# create an instance of BatchSendShipments200ResponseResultsInner from a JSON string
batch_send_shipments200_response_results_inner_instance = BatchSendShipments200ResponseResultsInner.from_json(json)
# print the JSON string representation of the object
print(BatchSendShipments200ResponseResultsInner.to_json())

# convert the object into a dict
batch_send_shipments200_response_results_inner_dict = batch_send_shipments200_response_results_inner_instance.to_dict()
# create an instance of BatchSendShipments200ResponseResultsInner from a dict
batch_send_shipments200_response_results_inner_from_dict = BatchSendShipments200ResponseResultsInner.from_dict(batch_send_shipments200_response_results_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


