# UpdateApiTokenRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** | New token name | 

## Example

```python
from zippendo.models.update_api_token_request import UpdateApiTokenRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateApiTokenRequest from a JSON string
update_api_token_request_instance = UpdateApiTokenRequest.from_json(json)
# print the JSON string representation of the object
print(UpdateApiTokenRequest.to_json())

# convert the object into a dict
update_api_token_request_dict = update_api_token_request_instance.to_dict()
# create an instance of UpdateApiTokenRequest from a dict
update_api_token_request_from_dict = UpdateApiTokenRequest.from_dict(update_api_token_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


