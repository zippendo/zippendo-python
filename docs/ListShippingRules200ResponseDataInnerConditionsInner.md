# ListShippingRules200ResponseDataInnerConditionsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** | Condition type discriminator | 
**min** | **float** | Minimum cart value (inclusive) | 
**max** | **float** | Maximum cart value (inclusive) | 
**shipping_price** | **float** | Flat shipping price | 
**currency** | **str** | ISO 4217 currency code | 
**price_type** | **str** | Whether to compare against subtotal (before discounts) or total (after discounts) | [default to 'total']
**operator** | **str** | Comparison operator | 
**value** | **int** | Quantity value to compare against | 

## Example

```python
from zippendo.models.list_shipping_rules200_response_data_inner_conditions_inner import ListShippingRules200ResponseDataInnerConditionsInner

# TODO update the JSON string below
json = "{}"
# create an instance of ListShippingRules200ResponseDataInnerConditionsInner from a JSON string
list_shipping_rules200_response_data_inner_conditions_inner_instance = ListShippingRules200ResponseDataInnerConditionsInner.from_json(json)
# print the JSON string representation of the object
print(ListShippingRules200ResponseDataInnerConditionsInner.to_json())

# convert the object into a dict
list_shipping_rules200_response_data_inner_conditions_inner_dict = list_shipping_rules200_response_data_inner_conditions_inner_instance.to_dict()
# create an instance of ListShippingRules200ResponseDataInnerConditionsInner from a dict
list_shipping_rules200_response_data_inner_conditions_inner_from_dict = ListShippingRules200ResponseDataInnerConditionsInner.from_dict(list_shipping_rules200_response_data_inner_conditions_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


