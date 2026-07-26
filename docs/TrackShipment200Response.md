# TrackShipment200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tracking_number** | **str** | Carrier tracking number. | 
**tracking_url** | **str** | Public carrier tracking URL. | 
**current_status** | **str** | Latest normalized tracking status. | 
**estimated_delivery** | **str** | Estimated delivery timestamp. | [optional] 
**events** | [**List[TrackShipment200ResponseEventsInner]**](TrackShipment200ResponseEventsInner.md) | Tracking events ordered from newest to oldest. | 

## Example

```python
from zippendo.models.track_shipment200_response import TrackShipment200Response

# TODO update the JSON string below
json = "{}"
# create an instance of TrackShipment200Response from a JSON string
track_shipment200_response_instance = TrackShipment200Response.from_json(json)
# print the JSON string representation of the object
print(TrackShipment200Response.to_json())

# convert the object into a dict
track_shipment200_response_dict = track_shipment200_response_instance.to_dict()
# create an instance of TrackShipment200Response from a dict
track_shipment200_response_from_dict = TrackShipment200Response.from_dict(track_shipment200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


