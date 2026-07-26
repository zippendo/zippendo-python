# GetBillingUsage200ResponseCurrentPeriod


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**start** | **str** | Start of the current usage period (ISO 8601) | 
**end** | **str** | End of the current usage period (ISO 8601) | 

## Example

```python
from zippendo.models.get_billing_usage200_response_current_period import GetBillingUsage200ResponseCurrentPeriod

# TODO update the JSON string below
json = "{}"
# create an instance of GetBillingUsage200ResponseCurrentPeriod from a JSON string
get_billing_usage200_response_current_period_instance = GetBillingUsage200ResponseCurrentPeriod.from_json(json)
# print the JSON string representation of the object
print(GetBillingUsage200ResponseCurrentPeriod.to_json())

# convert the object into a dict
get_billing_usage200_response_current_period_dict = get_billing_usage200_response_current_period_instance.to_dict()
# create an instance of GetBillingUsage200ResponseCurrentPeriod from a dict
get_billing_usage200_response_current_period_from_dict = GetBillingUsage200ResponseCurrentPeriod.from_dict(get_billing_usage200_response_current_period_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


