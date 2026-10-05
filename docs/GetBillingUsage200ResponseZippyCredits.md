# GetBillingUsage200ResponseZippyCredits

Zippy credit usage this period (present when the Zippy add-on is enabled)

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**used** | **float** | Zippy credits used this period, included bundle and metered alike | 
**included** | **float** | Credits included in the add-on bundle this period | 
**billed** | **float** | Credits beyond the bundle, metered this period | 
**charges** | **float** | Metered credit charges so far, in øre (whole packs) | 
**limit** | **float** | Maximum Zippy credits per month (-1 for unlimited) | 

## Example

```python
from zippendo.models.get_billing_usage200_response_zippy_credits import GetBillingUsage200ResponseZippyCredits

# TODO update the JSON string below
json = "{}"
# create an instance of GetBillingUsage200ResponseZippyCredits from a JSON string
get_billing_usage200_response_zippy_credits_instance = GetBillingUsage200ResponseZippyCredits.from_json(json)
# print the JSON string representation of the object
print(GetBillingUsage200ResponseZippyCredits.to_json())

# convert the object into a dict
get_billing_usage200_response_zippy_credits_dict = get_billing_usage200_response_zippy_credits_instance.to_dict()
# create an instance of GetBillingUsage200ResponseZippyCredits from a dict
get_billing_usage200_response_zippy_credits_from_dict = GetBillingUsage200ResponseZippyCredits.from_dict(get_billing_usage200_response_zippy_credits_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


