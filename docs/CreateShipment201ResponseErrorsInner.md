# CreateShipment201ResponseErrorsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | Unique error identifier. | 
**carrier** | **str** | Carrier that produced the error. | 
**code** | **str** | Carrier-specific error code. | [optional] 
**message** | **str** | Human-readable error message. | 
**created_at** | **str** | Timestamp when the error occurred. | 

## Example

```python
from zippendo.models.create_shipment201_response_errors_inner import CreateShipment201ResponseErrorsInner

# TODO update the JSON string below
json = "{}"
# create an instance of CreateShipment201ResponseErrorsInner from a JSON string
create_shipment201_response_errors_inner_instance = CreateShipment201ResponseErrorsInner.from_json(json)
# print the JSON string representation of the object
print(CreateShipment201ResponseErrorsInner.to_json())

# convert the object into a dict
create_shipment201_response_errors_inner_dict = create_shipment201_response_errors_inner_instance.to_dict()
# create an instance of CreateShipment201ResponseErrorsInner from a dict
create_shipment201_response_errors_inner_from_dict = CreateShipment201ResponseErrorsInner.from_dict(create_shipment201_response_errors_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


