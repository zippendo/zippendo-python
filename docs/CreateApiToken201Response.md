# CreateApiToken201Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | Unique API token identifier | 
**name** | **str** | Token name for identification | 
**token_prefix** | **str** | First 12 chars of the token for identification | 
**scopes** | **List[str]** | Permission scopes granted by the token | 
**brand_id** | **str** | Brand this token is restricted to, or null for organization-wide access | 
**last_used_at** | **str** | Timestamp the token was last used (ISO 8601), null if never used | 
**expires_at** | **str** | Expiry timestamp (ISO 8601), null if it never expires | 
**created_at** | **str** | Creation timestamp (ISO 8601) | 
**token** | **str** | Full API token (only shown once) | 

## Example

```python
from zippendo.models.create_api_token201_response import CreateApiToken201Response

# TODO update the JSON string below
json = "{}"
# create an instance of CreateApiToken201Response from a JSON string
create_api_token201_response_instance = CreateApiToken201Response.from_json(json)
# print the JSON string representation of the object
print(CreateApiToken201Response.to_json())

# convert the object into a dict
create_api_token201_response_dict = create_api_token201_response_instance.to_dict()
# create an instance of CreateApiToken201Response from a dict
create_api_token201_response_from_dict = CreateApiToken201Response.from_dict(create_api_token201_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


