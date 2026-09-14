# GetOrder200ResponseOrderLinesInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**sku** | **str** | Stock keeping unit identifier. | [optional] 
**name** | **str** | Product name. | 
**quantity** | **int** | Quantity ordered. | 
**unit_price** | **float** | Price per unit. | [optional] 
**total_price** | **float** | Total price for the line. | [optional] 
**currency** | **str** | ISO 4217 currency code. | [optional] 
**weight** | **float** | Item weight in the given unit. | [optional] 
**weight_unit** | **str** | Unit of the weight value. | [optional] 
**variant_id** | **str** | Platform variant identifier. | [optional] 
**product_id** | **str** | Platform product identifier. | [optional] 
**image_url** | **str** | Product image URL. | [optional] 
**hs_code** | **str** | Harmonized System customs code (6-13 digits). | [optional] 
**country_of_origin** | **str** | ISO 3166-1 alpha-2 country of origin. | [optional] 
**province_of_origin** | **str** | ISO 3166-2 province of origin. | [optional] 
**barcode** | **str** | Item barcode (EAN/UPC). | [optional] 
**requires_shipping** | **bool** | Whether the item requires shipping. | [optional] 
**taxable** | **bool** | Whether the item is taxable. | [optional] 
**gift_card** | **bool** | Whether the item is a gift card. | [optional] 
**vendor** | **str** | Vendor or brand name. | [optional] 
**id** | **str** | Order line ID. Present once the line is a row. Absent for jsonb-only lines during the dual-write window — do not synthesise one, or an edit would re-point packed lines. | [optional] 
**packed_quantity** | **int** | Quantity already allocated to outbound shipments. | 

## Example

```python
from zippendo.models.get_order200_response_order_lines_inner import GetOrder200ResponseOrderLinesInner

# TODO update the JSON string below
json = "{}"
# create an instance of GetOrder200ResponseOrderLinesInner from a JSON string
get_order200_response_order_lines_inner_instance = GetOrder200ResponseOrderLinesInner.from_json(json)
# print the JSON string representation of the object
print(GetOrder200ResponseOrderLinesInner.to_json())

# convert the object into a dict
get_order200_response_order_lines_inner_dict = get_order200_response_order_lines_inner_instance.to_dict()
# create an instance of GetOrder200ResponseOrderLinesInner from a dict
get_order200_response_order_lines_inner_from_dict = GetOrder200ResponseOrderLinesInner.from_dict(get_order200_response_order_lines_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


