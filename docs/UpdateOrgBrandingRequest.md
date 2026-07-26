# UpdateOrgBrandingRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**primary_color** | **str** | Primary brand color (hex) — tints the document title and table headers | [optional] 
**secondary_color** | **str** | Secondary brand color (hex) — tints the subtitle, section headings, and totals accent | [optional] 

## Example

```python
from zippendo.models.update_org_branding_request import UpdateOrgBrandingRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateOrgBrandingRequest from a JSON string
update_org_branding_request_instance = UpdateOrgBrandingRequest.from_json(json)
# print the JSON string representation of the object
print(UpdateOrgBrandingRequest.to_json())

# convert the object into a dict
update_org_branding_request_dict = update_org_branding_request_instance.to_dict()
# create an instance of UpdateOrgBrandingRequest from a dict
update_org_branding_request_from_dict = UpdateOrgBrandingRequest.from_dict(update_org_branding_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


