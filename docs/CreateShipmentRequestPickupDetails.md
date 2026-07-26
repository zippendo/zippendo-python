# CreateShipmentRequestPickupDetails


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**var_date** | **str** | Requested pickup date (YYYY-MM-DD). | 
**var_from** | **str** | Requested earliest pickup time (HH:MM:SS). | 
**to** | **str** | Requested latest pickup time (HH:MM:SS). | 
**instruction** | **str** | Pickup instruction to the carrier. | [optional] 

## Example

```python
from zippendo.models.create_shipment_request_pickup_details import CreateShipmentRequestPickupDetails

# TODO update the JSON string below
json = "{}"
# create an instance of CreateShipmentRequestPickupDetails from a JSON string
create_shipment_request_pickup_details_instance = CreateShipmentRequestPickupDetails.from_json(json)
# print the JSON string representation of the object
print(CreateShipmentRequestPickupDetails.to_json())

# convert the object into a dict
create_shipment_request_pickup_details_dict = create_shipment_request_pickup_details_instance.to_dict()
# create an instance of CreateShipmentRequestPickupDetails from a dict
create_shipment_request_pickup_details_from_dict = CreateShipmentRequestPickupDetails.from_dict(create_shipment_request_pickup_details_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


