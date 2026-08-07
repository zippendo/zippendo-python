# CreateApiTokenRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** | Token name for identification | 
**scopes** | **List[str]** | Permission scopes for the token | 
**expires_in_days** | **int** | Token expiry in days (optional, max 365) | [optional] 
**brand_id** | **str** | Restrict this token to a single brand. Requests made with it can only read and write that brand&#39;s data. Omit for organization-wide access. | [optional] 

## Example

```python
from zippendo.models.create_api_token_request import CreateApiTokenRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateApiTokenRequest from a JSON string
create_api_token_request_instance = CreateApiTokenRequest.from_json(json)
# print the JSON string representation of the object
print(CreateApiTokenRequest.to_json())

# convert the object into a dict
create_api_token_request_dict = create_api_token_request_instance.to_dict()
# create an instance of CreateApiTokenRequest from a dict
create_api_token_request_from_dict = CreateApiTokenRequest.from_dict(create_api_token_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


