# ListShippingRules200ResponseDataInnerConditionsInnerOneOf


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
from zippendo.models.list_shipping_rules200_response_data_inner_conditions_inner_one_of import ListShippingRules200ResponseDataInnerConditionsInnerOneOf

# TODO update the JSON string below
json = "{}"
# create an instance of ListShippingRules200ResponseDataInnerConditionsInnerOneOf from a JSON string
list_shipping_rules200_response_data_inner_conditions_inner_one_of_instance = ListShippingRules200ResponseDataInnerConditionsInnerOneOf.from_json(json)
# print the JSON string representation of the object
print(ListShippingRules200ResponseDataInnerConditionsInnerOneOf.to_json())

# convert the object into a dict
list_shipping_rules200_response_data_inner_conditions_inner_one_of_dict = list_shipping_rules200_response_data_inner_conditions_inner_one_of_instance.to_dict()
# create an instance of ListShippingRules200ResponseDataInnerConditionsInnerOneOf from a dict
list_shipping_rules200_response_data_inner_conditions_inner_one_of_from_dict = ListShippingRules200ResponseDataInnerConditionsInnerOneOf.from_dict(list_shipping_rules200_response_data_inner_conditions_inner_one_of_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


