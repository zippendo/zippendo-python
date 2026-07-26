# SplitShipmentParcel200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**shipment** | [**CreateShipment201Response**](CreateShipment201Response.md) |  | 

## Example

```python
from zippendo.models.split_shipment_parcel200_response import SplitShipmentParcel200Response

# TODO update the JSON string below
json = "{}"
# create an instance of SplitShipmentParcel200Response from a JSON string
split_shipment_parcel200_response_instance = SplitShipmentParcel200Response.from_json(json)
# print the JSON string representation of the object
print(SplitShipmentParcel200Response.to_json())

# convert the object into a dict
split_shipment_parcel200_response_dict = split_shipment_parcel200_response_instance.to_dict()
# create an instance of SplitShipmentParcel200Response from a dict
split_shipment_parcel200_response_from_dict = SplitShipmentParcel200Response.from_dict(split_shipment_parcel200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


