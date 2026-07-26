# CreateShipment201ResponseActivitiesInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | Unique activity identifier. | 
**action** | **str** | Type of activity performed on the shipment. | 
**description** | **str** | Human-readable description of the activity. | 
**metadata** | **object** | Additional structured data about the activity. | [optional] 
**created_at** | **str** | Timestamp when the activity occurred. | 

## Example

```python
from zippendo.models.create_shipment201_response_activities_inner import CreateShipment201ResponseActivitiesInner

# TODO update the JSON string below
json = "{}"
# create an instance of CreateShipment201ResponseActivitiesInner from a JSON string
create_shipment201_response_activities_inner_instance = CreateShipment201ResponseActivitiesInner.from_json(json)
# print the JSON string representation of the object
print(CreateShipment201ResponseActivitiesInner.to_json())

# convert the object into a dict
create_shipment201_response_activities_inner_dict = create_shipment201_response_activities_inner_instance.to_dict()
# create an instance of CreateShipment201ResponseActivitiesInner from a dict
create_shipment201_response_activities_inner_from_dict = CreateShipment201ResponseActivitiesInner.from_dict(create_shipment201_response_activities_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


