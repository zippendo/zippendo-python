# CreateShipment201ResponseLogsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | Unique log entry identifier. | 
**direction** | **str** | Direction of the logged request. | 
**request** | **object** | Captured request payload. | 
**response** | **object** | Captured response payload. | [optional] 
**status_code** | **float** | HTTP status code of the response. | [optional] 
**error** | **str** | Error message if the request failed. | [optional] 
**duration** | **float** | Request duration in milliseconds. | [optional] 
**created_at** | **str** | Timestamp when the log entry was created. | 

## Example

```python
from zippendo.models.create_shipment201_response_logs_inner import CreateShipment201ResponseLogsInner

# TODO update the JSON string below
json = "{}"
# create an instance of CreateShipment201ResponseLogsInner from a JSON string
create_shipment201_response_logs_inner_instance = CreateShipment201ResponseLogsInner.from_json(json)
# print the JSON string representation of the object
print(CreateShipment201ResponseLogsInner.to_json())

# convert the object into a dict
create_shipment201_response_logs_inner_dict = create_shipment201_response_logs_inner_instance.to_dict()
# create an instance of CreateShipment201ResponseLogsInner from a dict
create_shipment201_response_logs_inner_from_dict = CreateShipment201ResponseLogsInner.from_dict(create_shipment201_response_logs_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


