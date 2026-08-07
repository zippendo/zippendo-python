# ListApiTokens200ResponseDataInner


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
**created_by** | [**ListApiTokens200ResponseDataInnerCreatedBy**](ListApiTokens200ResponseDataInnerCreatedBy.md) |  | 

## Example

```python
from zippendo.models.list_api_tokens200_response_data_inner import ListApiTokens200ResponseDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of ListApiTokens200ResponseDataInner from a JSON string
list_api_tokens200_response_data_inner_instance = ListApiTokens200ResponseDataInner.from_json(json)
# print the JSON string representation of the object
print(ListApiTokens200ResponseDataInner.to_json())

# convert the object into a dict
list_api_tokens200_response_data_inner_dict = list_api_tokens200_response_data_inner_instance.to_dict()
# create an instance of ListApiTokens200ResponseDataInner from a dict
list_api_tokens200_response_data_inner_from_dict = ListApiTokens200ResponseDataInner.from_dict(list_api_tokens200_response_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


