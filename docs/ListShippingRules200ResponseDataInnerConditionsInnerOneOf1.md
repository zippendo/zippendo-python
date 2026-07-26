# ListShippingRules200ResponseDataInnerConditionsInnerOneOf1


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** | Condition type discriminator | 
**price_type** | **str** | Whether to compare against subtotal (before discounts) or total (after discounts) | [default to 'total']
**operator** | **str** | Comparison operator | 
**value** | **float** | Price value to compare against | 
**shipping_price** | **float** | Shipping price when condition matches | 
**currency** | **str** | ISO 4217 currency code | 

## Example

```python
from zippendo.models.list_shipping_rules200_response_data_inner_conditions_inner_one_of1 import ListShippingRules200ResponseDataInnerConditionsInnerOneOf1

# TODO update the JSON string below
json = "{}"
# create an instance of ListShippingRules200ResponseDataInnerConditionsInnerOneOf1 from a JSON string
list_shipping_rules200_response_data_inner_conditions_inner_one_of1_instance = ListShippingRules200ResponseDataInnerConditionsInnerOneOf1.from_json(json)
# print the JSON string representation of the object
print(ListShippingRules200ResponseDataInnerConditionsInnerOneOf1.to_json())

# convert the object into a dict
list_shipping_rules200_response_data_inner_conditions_inner_one_of1_dict = list_shipping_rules200_response_data_inner_conditions_inner_one_of1_instance.to_dict()
# create an instance of ListShippingRules200ResponseDataInnerConditionsInnerOneOf1 from a dict
list_shipping_rules200_response_data_inner_conditions_inner_one_of1_from_dict = ListShippingRules200ResponseDataInnerConditionsInnerOneOf1.from_dict(list_shipping_rules200_response_data_inner_conditions_inner_one_of1_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


