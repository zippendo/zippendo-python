# TrackShipment200ResponseEventsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | Unique tracking event identifier. | 
**status** | **str** | Normalized tracking status for the event. | 
**carrier_status** | **str** | Raw status string reported by the carrier. | 
**description** | **str** | Human-readable description of the event. | 
**location** | **str** | Location where the event was registered. | 
**occurred_at** | **str** | Timestamp when the event occurred. | 

## Example

```python
from zippendo.models.track_shipment200_response_events_inner import TrackShipment200ResponseEventsInner

# TODO update the JSON string below
json = "{}"
# create an instance of TrackShipment200ResponseEventsInner from a JSON string
track_shipment200_response_events_inner_instance = TrackShipment200ResponseEventsInner.from_json(json)
# print the JSON string representation of the object
print(TrackShipment200ResponseEventsInner.to_json())

# convert the object into a dict
track_shipment200_response_events_inner_dict = track_shipment200_response_events_inner_instance.to_dict()
# create an instance of TrackShipment200ResponseEventsInner from a dict
track_shipment200_response_events_inner_from_dict = TrackShipment200ResponseEventsInner.from_dict(track_shipment200_response_events_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


