# ListAvailableCarriers200ResponseInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** | Display name of the carrier | 
**slug** | **str** | Unique carrier slug identifier | 
**group** | **str** | Carrier group or family name | [optional] 
**description** | **str** | Short description of the carrier | [optional] 
**logo** | **str** | URL to the carrier logo image | [optional] 
**brand_color** | **str** | Carrier brand color (hex) | [optional] 
**learn_more_url** | **str** | URL with more information about the carrier | [optional] 
**required_fields** | [**List[ListAvailableCarriers200ResponseInnerRequiredFieldsInner]**](ListAvailableCarriers200ResponseInnerRequiredFieldsInner.md) | Configuration fields that must be provided to connect the carrier | [optional] 
**optional_fields** | [**List[ListAvailableCarriers200ResponseInnerRequiredFieldsInner]**](ListAvailableCarriers200ResponseInnerRequiredFieldsInner.md) | Optional configuration fields for the carrier | [optional] 
**deprecated** | **bool** | Whether this integration is deprecated (still works, but discouraged) | [optional] 
**deprecation_message** | **str** | Guidance shown alongside the deprecated tag (e.g. what to migrate to) | [optional] 

## Example

```python
from zippendo.models.list_available_carriers200_response_inner import ListAvailableCarriers200ResponseInner

# TODO update the JSON string below
json = "{}"
# create an instance of ListAvailableCarriers200ResponseInner from a JSON string
list_available_carriers200_response_inner_instance = ListAvailableCarriers200ResponseInner.from_json(json)
# print the JSON string representation of the object
print(ListAvailableCarriers200ResponseInner.to_json())

# convert the object into a dict
list_available_carriers200_response_inner_dict = list_available_carriers200_response_inner_instance.to_dict()
# create an instance of ListAvailableCarriers200ResponseInner from a dict
list_available_carriers200_response_inner_from_dict = ListAvailableCarriers200ResponseInner.from_dict(list_available_carriers200_response_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


