# GetBillingUsage200ResponseAddOnsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** | Type of billing add-on | 
**quantity** | **float** | Number of add-on units purchased | 
**unit_price** | **float** | Price per unit per month, in øre | 
**total_price** | **float** | Total price per month, in øre | 

## Example

```python
from zippendo.models.get_billing_usage200_response_add_ons_inner import GetBillingUsage200ResponseAddOnsInner

# TODO update the JSON string below
json = "{}"
# create an instance of GetBillingUsage200ResponseAddOnsInner from a JSON string
get_billing_usage200_response_add_ons_inner_instance = GetBillingUsage200ResponseAddOnsInner.from_json(json)
# print the JSON string representation of the object
print(GetBillingUsage200ResponseAddOnsInner.to_json())

# convert the object into a dict
get_billing_usage200_response_add_ons_inner_dict = get_billing_usage200_response_add_ons_inner_instance.to_dict()
# create an instance of GetBillingUsage200ResponseAddOnsInner from a dict
get_billing_usage200_response_add_ons_inner_from_dict = GetBillingUsage200ResponseAddOnsInner.from_dict(get_billing_usage200_response_add_ons_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


