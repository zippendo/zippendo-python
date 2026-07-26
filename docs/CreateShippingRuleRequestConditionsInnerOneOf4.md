# CreateShippingRuleRequestConditionsInnerOneOf4


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** | Condition type discriminator | 
**shipping_price** | **float** | Flat shipping price | 
**currency** | **str** | ISO 4217 currency code | 

## Example

```python
from zippendo.models.create_shipping_rule_request_conditions_inner_one_of4 import CreateShippingRuleRequestConditionsInnerOneOf4

# TODO update the JSON string below
json = "{}"
# create an instance of CreateShippingRuleRequestConditionsInnerOneOf4 from a JSON string
create_shipping_rule_request_conditions_inner_one_of4_instance = CreateShippingRuleRequestConditionsInnerOneOf4.from_json(json)
# print the JSON string representation of the object
print(CreateShippingRuleRequestConditionsInnerOneOf4.to_json())

# convert the object into a dict
create_shipping_rule_request_conditions_inner_one_of4_dict = create_shipping_rule_request_conditions_inner_one_of4_instance.to_dict()
# create an instance of CreateShippingRuleRequestConditionsInnerOneOf4 from a dict
create_shipping_rule_request_conditions_inner_one_of4_from_dict = CreateShippingRuleRequestConditionsInnerOneOf4.from_dict(create_shipping_rule_request_conditions_inner_one_of4_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


