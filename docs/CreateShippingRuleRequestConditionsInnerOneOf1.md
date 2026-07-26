# CreateShippingRuleRequestConditionsInnerOneOf1


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** | Condition type discriminator | 
**price_type** | **str** | Whether to compare against subtotal (before discounts) or total (after discounts) | [optional] [default to 'total']
**operator** | **str** | Comparison operator | 
**value** | **float** | Price value to compare against | 
**shipping_price** | **float** | Shipping price when condition matches | 
**currency** | **str** | ISO 4217 currency code | 

## Example

```python
from zippendo.models.create_shipping_rule_request_conditions_inner_one_of1 import CreateShippingRuleRequestConditionsInnerOneOf1

# TODO update the JSON string below
json = "{}"
# create an instance of CreateShippingRuleRequestConditionsInnerOneOf1 from a JSON string
create_shipping_rule_request_conditions_inner_one_of1_instance = CreateShippingRuleRequestConditionsInnerOneOf1.from_json(json)
# print the JSON string representation of the object
print(CreateShippingRuleRequestConditionsInnerOneOf1.to_json())

# convert the object into a dict
create_shipping_rule_request_conditions_inner_one_of1_dict = create_shipping_rule_request_conditions_inner_one_of1_instance.to_dict()
# create an instance of CreateShippingRuleRequestConditionsInnerOneOf1 from a dict
create_shipping_rule_request_conditions_inner_one_of1_from_dict = CreateShippingRuleRequestConditionsInnerOneOf1.from_dict(create_shipping_rule_request_conditions_inner_one_of1_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


