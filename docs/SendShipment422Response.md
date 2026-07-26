# SendShipment422Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **str** | Machine-readable error code. | [optional] 
**error** | **str** | Error category. | 
**message** | **str** | Human-readable summary of the carrier failure. | 
**errors** | [**List[SendShipment422ResponseErrorsInner]**](SendShipment422ResponseErrorsInner.md) | Detailed carrier errors that caused the booking to fail. | 

## Example

```python
from zippendo.models.send_shipment422_response import SendShipment422Response

# TODO update the JSON string below
json = "{}"
# create an instance of SendShipment422Response from a JSON string
send_shipment422_response_instance = SendShipment422Response.from_json(json)
# print the JSON string representation of the object
print(SendShipment422Response.to_json())

# convert the object into a dict
send_shipment422_response_dict = send_shipment422_response_instance.to_dict()
# create an instance of SendShipment422Response from a dict
send_shipment422_response_from_dict = SendShipment422Response.from_dict(send_shipment422_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


