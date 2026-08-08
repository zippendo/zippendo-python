# CheckBrandSlug200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**slug** | **str** | The slug that was checked | 
**available** | **bool** | Whether the slug is free within this organization | 

## Example

```python
from zippendo.models.check_brand_slug200_response import CheckBrandSlug200Response

# TODO update the JSON string below
json = "{}"
# create an instance of CheckBrandSlug200Response from a JSON string
check_brand_slug200_response_instance = CheckBrandSlug200Response.from_json(json)
# print the JSON string representation of the object
print(CheckBrandSlug200Response.to_json())

# convert the object into a dict
check_brand_slug200_response_dict = check_brand_slug200_response_instance.to_dict()
# create an instance of CheckBrandSlug200Response from a dict
check_brand_slug200_response_from_dict = CheckBrandSlug200Response.from_dict(check_brand_slug200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


