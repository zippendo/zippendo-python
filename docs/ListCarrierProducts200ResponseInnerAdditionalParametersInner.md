# ListCarrierProducts200ResponseInnerAdditionalParametersInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** | Display label for the parameter | 
**key** | **str** | Machine key the value is stored under | 
**type** | **str** | Data type of the parameter | 
**options** | [**List[ListCarrierProducts200ResponseInnerAdditionalParametersInnerOptionsInner]**](ListCarrierProducts200ResponseInnerAdditionalParametersInnerOptionsInner.md) | Selectable options for enum-type parameters | [optional] 
**description** | **str** | Description of the parameter | 
**is_required** | **bool** | Whether the parameter is mandatory | [default to False]
**required_service** | **List[str]** | Service IDs for which this parameter is required | [optional] 

## Example

```python
from zippendo.models.list_carrier_products200_response_inner_additional_parameters_inner import ListCarrierProducts200ResponseInnerAdditionalParametersInner

# TODO update the JSON string below
json = "{}"
# create an instance of ListCarrierProducts200ResponseInnerAdditionalParametersInner from a JSON string
list_carrier_products200_response_inner_additional_parameters_inner_instance = ListCarrierProducts200ResponseInnerAdditionalParametersInner.from_json(json)
# print the JSON string representation of the object
print(ListCarrierProducts200ResponseInnerAdditionalParametersInner.to_json())

# convert the object into a dict
list_carrier_products200_response_inner_additional_parameters_inner_dict = list_carrier_products200_response_inner_additional_parameters_inner_instance.to_dict()
# create an instance of ListCarrierProducts200ResponseInnerAdditionalParametersInner from a dict
list_carrier_products200_response_inner_additional_parameters_inner_from_dict = ListCarrierProducts200ResponseInnerAdditionalParametersInner.from_dict(list_carrier_products200_response_inner_additional_parameters_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


