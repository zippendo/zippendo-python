# CreateShippingRuleRequestAdditionalParameters

Carrier-specific extra parameters. Accepts EITHER the `{ key: value }` object (preferred) OR the legacy `[{ name, val }]` array, so you can migrate on your own schedule. Each key / `name` is the carrier parameter `key` from the product's `additionalParameters[].key` (e.g. `returnFunctionality`).

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------

## Example

```python
from zippendo.models.create_shipping_rule_request_additional_parameters import CreateShippingRuleRequestAdditionalParameters

# TODO update the JSON string below
json = "{}"
# create an instance of CreateShippingRuleRequestAdditionalParameters from a JSON string
create_shipping_rule_request_additional_parameters_instance = CreateShippingRuleRequestAdditionalParameters.from_json(json)
# print the JSON string representation of the object
print(CreateShippingRuleRequestAdditionalParameters.to_json())

# convert the object into a dict
create_shipping_rule_request_additional_parameters_dict = create_shipping_rule_request_additional_parameters_instance.to_dict()
# create an instance of CreateShippingRuleRequestAdditionalParameters from a dict
create_shipping_rule_request_additional_parameters_from_dict = CreateShippingRuleRequestAdditionalParameters.from_dict(create_shipping_rule_request_additional_parameters_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


