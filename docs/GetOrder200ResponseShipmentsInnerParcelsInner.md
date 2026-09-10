# GetOrder200ResponseShipmentsInnerParcelsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | Parcel ID. | 
**weight** | **float** | Parcel weight in the given unit. | 
**weight_unit** | **str** | Unit of measurement for parcel weight. | 
**dimensions** | [**CreateShipment201ResponseParcelsInnerDimensions**](CreateShipment201ResponseParcelsInnerDimensions.md) |  | 
**order_lines** | [**List[GetOrder200ResponseShipmentsInnerParcelsInnerOrderLinesInner]**](GetOrder200ResponseShipmentsInnerParcelsInnerOrderLinesInner.md) | Contents of this parcel. | 

## Example

```python
from zippendo.models.get_order200_response_shipments_inner_parcels_inner import GetOrder200ResponseShipmentsInnerParcelsInner

# TODO update the JSON string below
json = "{}"
# create an instance of GetOrder200ResponseShipmentsInnerParcelsInner from a JSON string
get_order200_response_shipments_inner_parcels_inner_instance = GetOrder200ResponseShipmentsInnerParcelsInner.from_json(json)
# print the JSON string representation of the object
print(GetOrder200ResponseShipmentsInnerParcelsInner.to_json())

# convert the object into a dict
get_order200_response_shipments_inner_parcels_inner_dict = get_order200_response_shipments_inner_parcels_inner_instance.to_dict()
# create an instance of GetOrder200ResponseShipmentsInnerParcelsInner from a dict
get_order200_response_shipments_inner_parcels_inner_from_dict = GetOrder200ResponseShipmentsInnerParcelsInner.from_dict(get_order200_response_shipments_inner_parcels_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


