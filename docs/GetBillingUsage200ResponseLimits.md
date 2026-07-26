# GetBillingUsage200ResponseLimits


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**team_members** | [**GetBillingUsage200ResponseLimitsTeamMembers**](GetBillingUsage200ResponseLimitsTeamMembers.md) |  | 
**carriers** | [**GetBillingUsage200ResponseLimitsTeamMembers**](GetBillingUsage200ResponseLimitsTeamMembers.md) |  | 
**order_channels** | [**GetBillingUsage200ResponseLimitsTeamMembers**](GetBillingUsage200ResponseLimitsTeamMembers.md) |  | 
**shipping_rules** | [**GetBillingUsage200ResponseLimitsTeamMembers**](GetBillingUsage200ResponseLimitsTeamMembers.md) |  | 
**addresses** | [**GetBillingUsage200ResponseLimitsTeamMembers**](GetBillingUsage200ResponseLimitsTeamMembers.md) |  | 
**api_tokens** | [**GetBillingUsage200ResponseLimitsTeamMembers**](GetBillingUsage200ResponseLimitsTeamMembers.md) |  | 
**automations** | [**GetBillingUsage200ResponseLimitsTeamMembers**](GetBillingUsage200ResponseLimitsTeamMembers.md) |  | 

## Example

```python
from zippendo.models.get_billing_usage200_response_limits import GetBillingUsage200ResponseLimits

# TODO update the JSON string below
json = "{}"
# create an instance of GetBillingUsage200ResponseLimits from a JSON string
get_billing_usage200_response_limits_instance = GetBillingUsage200ResponseLimits.from_json(json)
# print the JSON string representation of the object
print(GetBillingUsage200ResponseLimits.to_json())

# convert the object into a dict
get_billing_usage200_response_limits_dict = get_billing_usage200_response_limits_instance.to_dict()
# create an instance of GetBillingUsage200ResponseLimits from a dict
get_billing_usage200_response_limits_from_dict = GetBillingUsage200ResponseLimits.from_dict(get_billing_usage200_response_limits_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


