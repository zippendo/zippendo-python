# GetBillingUsage200ResponseLimitsTeamMembers


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**used** | **float** | Amount of the resource currently used | 
**limit** | **float** | Maximum allowed (-1 for unlimited) | 

## Example

```python
from zippendo.models.get_billing_usage200_response_limits_team_members import GetBillingUsage200ResponseLimitsTeamMembers

# TODO update the JSON string below
json = "{}"
# create an instance of GetBillingUsage200ResponseLimitsTeamMembers from a JSON string
get_billing_usage200_response_limits_team_members_instance = GetBillingUsage200ResponseLimitsTeamMembers.from_json(json)
# print the JSON string representation of the object
print(GetBillingUsage200ResponseLimitsTeamMembers.to_json())

# convert the object into a dict
get_billing_usage200_response_limits_team_members_dict = get_billing_usage200_response_limits_team_members_instance.to_dict()
# create an instance of GetBillingUsage200ResponseLimitsTeamMembers from a dict
get_billing_usage200_response_limits_team_members_from_dict = GetBillingUsage200ResponseLimitsTeamMembers.from_dict(get_billing_usage200_response_limits_team_members_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


