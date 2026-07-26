# VerifyApiTokenRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**token** | **str** | The API token to verify | 

## Example

```python
from zippendo.models.verify_api_token_request import VerifyApiTokenRequest

# TODO update the JSON string below
json = "{}"
# create an instance of VerifyApiTokenRequest from a JSON string
verify_api_token_request_instance = VerifyApiTokenRequest.from_json(json)
# print the JSON string representation of the object
print(VerifyApiTokenRequest.to_json())

# convert the object into a dict
verify_api_token_request_dict = verify_api_token_request_instance.to_dict()
# create an instance of VerifyApiTokenRequest from a dict
verify_api_token_request_from_dict = VerifyApiTokenRequest.from_dict(verify_api_token_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


