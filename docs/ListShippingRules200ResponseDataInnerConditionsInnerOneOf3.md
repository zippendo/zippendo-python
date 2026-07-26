# ListShippingRules200ResponseDataInnerConditionsInnerOneOf3


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** | Condition type discriminator | 
**operator** | **str** | Comparison operator | 
**value** | **int** | Quantity value to compare against | 
**shipping_price** | **float** | Shipping price when condition matches | 
**currency** | **str** | ISO 4217 currency code | 

## Example

```python
from zippendo.models.list_shipping_rules200_response_data_inner_conditions_inner_one_of3 import ListShippingRules200ResponseDataInnerConditionsInnerOneOf3

# TODO update the JSON string below
json = "{}"
# create an instance of ListShippingRules200ResponseDataInnerConditionsInnerOneOf3 from a JSON string
list_shipping_rules200_response_data_inner_conditions_inner_one_of3_instance = ListShippingRules200ResponseDataInnerConditionsInnerOneOf3.from_json(json)
# print the JSON string representation of the object
print(ListShippingRules200ResponseDataInnerConditionsInnerOneOf3.to_json())

# convert the object into a dict
list_shipping_rules200_response_data_inner_conditions_inner_one_of3_dict = list_shipping_rules200_response_data_inner_conditions_inner_one_of3_instance.to_dict()
# create an instance of ListShippingRules200ResponseDataInnerConditionsInnerOneOf3 from a dict
list_shipping_rules200_response_data_inner_conditions_inner_one_of3_from_dict = ListShippingRules200ResponseDataInnerConditionsInnerOneOf3.from_dict(list_shipping_rules200_response_data_inner_conditions_inner_one_of3_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


