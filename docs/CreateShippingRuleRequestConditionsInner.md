# CreateShippingRuleRequestConditionsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** | Condition type discriminator | 
**min** | **float** | Minimum cart value (inclusive) | 
**max** | **float** | Maximum cart value (inclusive) | 
**shipping_price** | **float** | Flat shipping price | 
**currency** | **str** | ISO 4217 currency code | 
**price_type** | **str** | Whether to compare against subtotal (before discounts) or total (after discounts) | [optional] [default to 'total']
**operator** | **str** | Comparison operator | 
**value** | **int** | Quantity value to compare against | 

## Example

```python
from zippendo.models.create_shipping_rule_request_conditions_inner import CreateShippingRuleRequestConditionsInner

# TODO update the JSON string below
json = "{}"
# create an instance of CreateShippingRuleRequestConditionsInner from a JSON string
create_shipping_rule_request_conditions_inner_instance = CreateShippingRuleRequestConditionsInner.from_json(json)
# print the JSON string representation of the object
print(CreateShippingRuleRequestConditionsInner.to_json())

# convert the object into a dict
create_shipping_rule_request_conditions_inner_dict = create_shipping_rule_request_conditions_inner_instance.to_dict()
# create an instance of CreateShippingRuleRequestConditionsInner from a dict
create_shipping_rule_request_conditions_inner_from_dict = CreateShippingRuleRequestConditionsInner.from_dict(create_shipping_rule_request_conditions_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


