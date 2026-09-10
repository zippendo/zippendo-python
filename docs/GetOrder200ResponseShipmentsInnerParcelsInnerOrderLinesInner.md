# GetOrder200ResponseShipmentsInnerParcelsInnerOrderLinesInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | Parcel content line ID. | 
**sku** | **str** | SKU of the packed item. | [optional] 
**quantity** | **int** | Quantity packed in this parcel. | 
**description** | **str** | Product description. | [optional] 

## Example

```python
from zippendo.models.get_order200_response_shipments_inner_parcels_inner_order_lines_inner import GetOrder200ResponseShipmentsInnerParcelsInnerOrderLinesInner

# TODO update the JSON string below
json = "{}"
# create an instance of GetOrder200ResponseShipmentsInnerParcelsInnerOrderLinesInner from a JSON string
get_order200_response_shipments_inner_parcels_inner_order_lines_inner_instance = GetOrder200ResponseShipmentsInnerParcelsInnerOrderLinesInner.from_json(json)
# print the JSON string representation of the object
print(GetOrder200ResponseShipmentsInnerParcelsInnerOrderLinesInner.to_json())

# convert the object into a dict
get_order200_response_shipments_inner_parcels_inner_order_lines_inner_dict = get_order200_response_shipments_inner_parcels_inner_order_lines_inner_instance.to_dict()
# create an instance of GetOrder200ResponseShipmentsInnerParcelsInnerOrderLinesInner from a dict
get_order200_response_shipments_inner_parcels_inner_order_lines_inner_from_dict = GetOrder200ResponseShipmentsInnerParcelsInnerOrderLinesInner.from_dict(get_order200_response_shipments_inner_parcels_inner_order_lines_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


