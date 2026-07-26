# ListApiTokens200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[ListApiTokens200ResponseDataInner]**](ListApiTokens200ResponseDataInner.md) | Page of results | 
**total** | **float** | Total matching items across all pages | 
**page** | **float** | Current page number (1-based) | 
**limit** | **float** | Items per page | 
**total_pages** | **float** | Total number of pages | 

## Example

```python
from zippendo.models.list_api_tokens200_response import ListApiTokens200Response

# TODO update the JSON string below
json = "{}"
# create an instance of ListApiTokens200Response from a JSON string
list_api_tokens200_response_instance = ListApiTokens200Response.from_json(json)
# print the JSON string representation of the object
print(ListApiTokens200Response.to_json())

# convert the object into a dict
list_api_tokens200_response_dict = list_api_tokens200_response_instance.to_dict()
# create an instance of ListApiTokens200Response from a dict
list_api_tokens200_response_from_dict = ListApiTokens200Response.from_dict(list_api_tokens200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


