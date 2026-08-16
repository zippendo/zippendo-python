# GetBillingUsage200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**current_period** | [**GetBillingUsage200ResponseCurrentPeriod**](GetBillingUsage200ResponseCurrentPeriod.md) |  | 
**shipments** | [**GetBillingUsage200ResponseShipments**](GetBillingUsage200ResponseShipments.md) |  | 
**limits** | [**GetBillingUsage200ResponseLimits**](GetBillingUsage200ResponseLimits.md) |  | 
**add_ons** | [**List[GetBillingUsage200ResponseAddOnsInner]**](GetBillingUsage200ResponseAddOnsInner.md) | Active add-ons on the subscription | 
**zippy_messages** | [**GetBillingUsage200ResponseZippyMessages**](GetBillingUsage200ResponseZippyMessages.md) |  | [optional] 

## Example

```python
from zippendo.models.get_billing_usage200_response import GetBillingUsage200Response

# TODO update the JSON string below
json = "{}"
# create an instance of GetBillingUsage200Response from a JSON string
get_billing_usage200_response_instance = GetBillingUsage200Response.from_json(json)
# print the JSON string representation of the object
print(GetBillingUsage200Response.to_json())

# convert the object into a dict
get_billing_usage200_response_dict = get_billing_usage200_response_instance.to_dict()
# create an instance of GetBillingUsage200Response from a dict
get_billing_usage200_response_from_dict = GetBillingUsage200Response.from_dict(get_billing_usage200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


