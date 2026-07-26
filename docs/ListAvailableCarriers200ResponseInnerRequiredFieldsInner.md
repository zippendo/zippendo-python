# ListAvailableCarriers200ResponseInnerRequiredFieldsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** | Human-readable label for the configuration field | 
**key** | **str** | Machine key used to store the field value | 
**type** | **str** | Data type of the configuration field | 
**options** | [**List[ListCarrierProducts200ResponseInnerAdditionalParametersInnerOptionsInner]**](ListCarrierProducts200ResponseInnerAdditionalParametersInnerOptionsInner.md) | Selectable options for enum-type fields | [optional] 
**description** | **str** | Help text describing the field | 
**required** | **bool** | Whether the field is mandatory | [optional] 

## Example

```python
from zippendo.models.list_available_carriers200_response_inner_required_fields_inner import ListAvailableCarriers200ResponseInnerRequiredFieldsInner

# TODO update the JSON string below
json = "{}"
# create an instance of ListAvailableCarriers200ResponseInnerRequiredFieldsInner from a JSON string
list_available_carriers200_response_inner_required_fields_inner_instance = ListAvailableCarriers200ResponseInnerRequiredFieldsInner.from_json(json)
# print the JSON string representation of the object
print(ListAvailableCarriers200ResponseInnerRequiredFieldsInner.to_json())

# convert the object into a dict
list_available_carriers200_response_inner_required_fields_inner_dict = list_available_carriers200_response_inner_required_fields_inner_instance.to_dict()
# create an instance of ListAvailableCarriers200ResponseInnerRequiredFieldsInner from a dict
list_available_carriers200_response_inner_required_fields_inner_from_dict = ListAvailableCarriers200ResponseInnerRequiredFieldsInner.from_dict(list_available_carriers200_response_inner_required_fields_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


