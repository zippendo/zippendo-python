# SendShipment422ResponseErrorsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **str** | Carrier-specific error code. | [optional] 
**message** | **str** | Carrier-specific error message. | 

## Example

```python
from zippendo.models.send_shipment422_response_errors_inner import SendShipment422ResponseErrorsInner

# TODO update the JSON string below
json = "{}"
# create an instance of SendShipment422ResponseErrorsInner from a JSON string
send_shipment422_response_errors_inner_instance = SendShipment422ResponseErrorsInner.from_json(json)
# print the JSON string representation of the object
print(SendShipment422ResponseErrorsInner.to_json())

# convert the object into a dict
send_shipment422_response_errors_inner_dict = send_shipment422_response_errors_inner_instance.to_dict()
# create an instance of SendShipment422ResponseErrorsInner from a dict
send_shipment422_response_errors_inner_from_dict = SendShipment422ResponseErrorsInner.from_dict(send_shipment422_response_errors_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


