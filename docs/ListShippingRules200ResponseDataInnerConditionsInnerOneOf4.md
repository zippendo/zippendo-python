# ListShippingRules200ResponseDataInnerConditionsInnerOneOf4


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** | Condition type discriminator | 
**shipping_price** | **float** | Flat shipping price | 
**currency** | **str** | ISO 4217 currency code | 

## Example

```python
from zippendo.models.list_shipping_rules200_response_data_inner_conditions_inner_one_of4 import ListShippingRules200ResponseDataInnerConditionsInnerOneOf4

# TODO update the JSON string below
json = "{}"
# create an instance of ListShippingRules200ResponseDataInnerConditionsInnerOneOf4 from a JSON string
list_shipping_rules200_response_data_inner_conditions_inner_one_of4_instance = ListShippingRules200ResponseDataInnerConditionsInnerOneOf4.from_json(json)
# print the JSON string representation of the object
print(ListShippingRules200ResponseDataInnerConditionsInnerOneOf4.to_json())

# convert the object into a dict
list_shipping_rules200_response_data_inner_conditions_inner_one_of4_dict = list_shipping_rules200_response_data_inner_conditions_inner_one_of4_instance.to_dict()
# create an instance of ListShippingRules200ResponseDataInnerConditionsInnerOneOf4 from a dict
list_shipping_rules200_response_data_inner_conditions_inner_one_of4_from_dict = ListShippingRules200ResponseDataInnerConditionsInnerOneOf4.from_dict(list_shipping_rules200_response_data_inner_conditions_inner_one_of4_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


