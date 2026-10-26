# CreateShippingRuleRequestTranslationsValue


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** | Checkout name in this language; blank keeps the rule&#39;s own name. | [optional] 
**description** | **str** | Checkout description in this language; blank keeps the rule&#39;s own description. | [optional] 

## Example

```python
from zippendo.models.create_shipping_rule_request_translations_value import CreateShippingRuleRequestTranslationsValue

# TODO update the JSON string below
json = "{}"
# create an instance of CreateShippingRuleRequestTranslationsValue from a JSON string
create_shipping_rule_request_translations_value_instance = CreateShippingRuleRequestTranslationsValue.from_json(json)
# print the JSON string representation of the object
print(CreateShippingRuleRequestTranslationsValue.to_json())

# convert the object into a dict
create_shipping_rule_request_translations_value_dict = create_shipping_rule_request_translations_value_instance.to_dict()
# create an instance of CreateShippingRuleRequestTranslationsValue from a dict
create_shipping_rule_request_translations_value_from_dict = CreateShippingRuleRequestTranslationsValue.from_dict(create_shipping_rule_request_translations_value_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


