# VerifyApiToken200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**valid** | **bool** | Whether the token is valid | 
**token_id** | **str** | Token identifier | [optional] 
**user_id** | **str** | User identifier the token belongs to | [optional] 
**org_id** | **str** | Organization identifier the token belongs to | [optional] 
**scopes** | **List[str]** | Permission scopes granted by the token | [optional] 
**expires_at** | **str** | Expiry timestamp (ISO 8601), null if it never expires | [optional] 

## Example

```python
from zippendo.models.verify_api_token200_response import VerifyApiToken200Response

# TODO update the JSON string below
json = "{}"
# create an instance of VerifyApiToken200Response from a JSON string
verify_api_token200_response_instance = VerifyApiToken200Response.from_json(json)
# print the JSON string representation of the object
print(VerifyApiToken200Response.to_json())

# convert the object into a dict
verify_api_token200_response_dict = verify_api_token200_response_instance.to_dict()
# create an instance of VerifyApiToken200Response from a dict
verify_api_token200_response_from_dict = VerifyApiToken200Response.from_dict(verify_api_token200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


