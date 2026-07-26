# CreateShipment201ResponsePickupDetails


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**var_date** | **str** | Requested pickup date (YYYY-MM-DD). | 
**var_from** | **str** | Requested earliest pickup time (HH:MM:SS). | 
**to** | **str** | Requested latest pickup time (HH:MM:SS). | 
**instruction** | **str** | Pickup instruction to the carrier. | [optional] 

## Example

```python
from zippendo.models.create_shipment201_response_pickup_details import CreateShipment201ResponsePickupDetails

# TODO update the JSON string below
json = "{}"
# create an instance of CreateShipment201ResponsePickupDetails from a JSON string
create_shipment201_response_pickup_details_instance = CreateShipment201ResponsePickupDetails.from_json(json)
# print the JSON string representation of the object
print(CreateShipment201ResponsePickupDetails.to_json())

# convert the object into a dict
create_shipment201_response_pickup_details_dict = create_shipment201_response_pickup_details_instance.to_dict()
# create an instance of CreateShipment201ResponsePickupDetails from a dict
create_shipment201_response_pickup_details_from_dict = CreateShipment201ResponsePickupDetails.from_dict(create_shipment201_response_pickup_details_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


