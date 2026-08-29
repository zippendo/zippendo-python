# GetBillingUsage200ResponseZippyMessages

Zippy AI message usage this period (present when Zippy access is enabled)

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**used** | **float** | Zippy messages used this period | 
**charges** | **float** | Zippy message charges so far, in øre | 
**limit** | **float** | Maximum Zippy messages per month (-1 for unlimited) | 

## Example

```python
from zippendo.models.get_billing_usage200_response_zippy_messages import GetBillingUsage200ResponseZippyMessages

# TODO update the JSON string below
json = "{}"
# create an instance of GetBillingUsage200ResponseZippyMessages from a JSON string
get_billing_usage200_response_zippy_messages_instance = GetBillingUsage200ResponseZippyMessages.from_json(json)
# print the JSON string representation of the object
print(GetBillingUsage200ResponseZippyMessages.to_json())

# convert the object into a dict
get_billing_usage200_response_zippy_messages_dict = get_billing_usage200_response_zippy_messages_instance.to_dict()
# create an instance of GetBillingUsage200ResponseZippyMessages from a dict
get_billing_usage200_response_zippy_messages_from_dict = GetBillingUsage200ResponseZippyMessages.from_dict(get_billing_usage200_response_zippy_messages_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


