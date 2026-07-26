# GetOrgBranding200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**primary_color** | **str** | Primary brand color (hex) | 
**secondary_color** | **str** | Secondary brand color (hex) | 
**logo_url** | **str** | Authenticated URL to download the org logo image, or null if no logo is set | 

## Example

```python
from zippendo.models.get_org_branding200_response import GetOrgBranding200Response

# TODO update the JSON string below
json = "{}"
# create an instance of GetOrgBranding200Response from a JSON string
get_org_branding200_response_instance = GetOrgBranding200Response.from_json(json)
# print the JSON string representation of the object
print(GetOrgBranding200Response.to_json())

# convert the object into a dict
get_org_branding200_response_dict = get_org_branding200_response_instance.to_dict()
# create an instance of GetOrgBranding200Response from a dict
get_org_branding200_response_from_dict = GetOrgBranding200Response.from_dict(get_org_branding200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


