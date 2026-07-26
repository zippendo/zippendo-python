# CreateShippingRuleRequestConditionsInnerOneOf


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** | Condition type discriminator | 
**min** | **float** | Minimum weight in kg (inclusive) | 
**max** | **float** | Maximum weight in kg (inclusive) | 
**shipping_price** | **float** | Shipping price when condition matches | 
**currency** | **str** | ISO 4217 currency code | 

## Example

```python
from zippendo.models.create_shipping_rule_request_conditions_inner_one_of import CreateShippingRuleRequestConditionsInnerOneOf

# TODO update the JSON string below
json = "{}"
# create an instance of CreateShippingRuleRequestConditionsInnerOneOf from a JSON string
create_shipping_rule_request_conditions_inner_one_of_instance = CreateShippingRuleRequestConditionsInnerOneOf.from_json(json)
# print the JSON string representation of the object
print(CreateShippingRuleRequestConditionsInnerOneOf.to_json())

# convert the object into a dict
create_shipping_rule_request_conditions_inner_one_of_dict = create_shipping_rule_request_conditions_inner_one_of_instance.to_dict()
# create an instance of CreateShippingRuleRequestConditionsInnerOneOf from a dict
create_shipping_rule_request_conditions_inner_one_of_from_dict = CreateShippingRuleRequestConditionsInnerOneOf.from_dict(create_shipping_rule_request_conditions_inner_one_of_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


