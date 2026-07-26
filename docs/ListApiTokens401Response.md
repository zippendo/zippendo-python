# ListApiTokens401Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **str** | Machine-readable error code (translate by this on the client) | [optional] 
**error** | **str** | Short human title | 
**message** | **str** | Human-readable English detail (i18n fallback) | 

## Example

```python
from zippendo.models.list_api_tokens401_response import ListApiTokens401Response

# TODO update the JSON string below
json = "{}"
# create an instance of ListApiTokens401Response from a JSON string
list_api_tokens401_response_instance = ListApiTokens401Response.from_json(json)
# print the JSON string representation of the object
print(ListApiTokens401Response.to_json())

# convert the object into a dict
list_api_tokens401_response_dict = list_api_tokens401_response_instance.to_dict()
# create an instance of ListApiTokens401Response from a dict
list_api_tokens401_response_from_dict = ListApiTokens401Response.from_dict(list_api_tokens401_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


