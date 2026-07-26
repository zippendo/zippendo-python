# CreateShippingQuoteRequestItemsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** | Item name | 
**sku** | **str** | SKU identifier | [optional] 
**quantity** | **int** | Quantity | 
**grams** | **float** | Weight in grams | 
**price** | **float** | Price in cents | 
**product_id** | **str** | Product ID | [optional] 
**variant_id** | **str** | Variant ID | [optional] 

## Example

```python
from zippendo.models.create_shipping_quote_request_items_inner import CreateShippingQuoteRequestItemsInner

# TODO update the JSON string below
json = "{}"
# create an instance of CreateShippingQuoteRequestItemsInner from a JSON string
create_shipping_quote_request_items_inner_instance = CreateShippingQuoteRequestItemsInner.from_json(json)
# print the JSON string representation of the object
print(CreateShippingQuoteRequestItemsInner.to_json())

# convert the object into a dict
create_shipping_quote_request_items_inner_dict = create_shipping_quote_request_items_inner_instance.to_dict()
# create an instance of CreateShippingQuoteRequestItemsInner from a dict
create_shipping_quote_request_items_inner_from_dict = CreateShippingQuoteRequestItemsInner.from_dict(create_shipping_quote_request_items_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


