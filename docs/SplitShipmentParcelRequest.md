# SplitShipmentParcelRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**parcels** | [**List[SplitShipmentParcelRequestParcelsInner]**](SplitShipmentParcelRequestParcelsInner.md) | Target parcel layout to redistribute order lines into. | 

## Example

```python
from zippendo.models.split_shipment_parcel_request import SplitShipmentParcelRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SplitShipmentParcelRequest from a JSON string
split_shipment_parcel_request_instance = SplitShipmentParcelRequest.from_json(json)
# print the JSON string representation of the object
print(SplitShipmentParcelRequest.to_json())

# convert the object into a dict
split_shipment_parcel_request_dict = split_shipment_parcel_request_instance.to_dict()
# create an instance of SplitShipmentParcelRequest from a dict
split_shipment_parcel_request_from_dict = SplitShipmentParcelRequest.from_dict(split_shipment_parcel_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


