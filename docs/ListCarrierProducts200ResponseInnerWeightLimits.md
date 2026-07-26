# ListCarrierProducts200ResponseInnerWeightLimits

Allowed weight range for parcels using this product

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**min** | **float** | Minimum allowed parcel weight | 
**max** | **float** | Maximum allowed parcel weight | 
**unit** | **str** | Unit of the weight limits | 

## Example

```python
from zippendo.models.list_carrier_products200_response_inner_weight_limits import ListCarrierProducts200ResponseInnerWeightLimits

# TODO update the JSON string below
json = "{}"
# create an instance of ListCarrierProducts200ResponseInnerWeightLimits from a JSON string
list_carrier_products200_response_inner_weight_limits_instance = ListCarrierProducts200ResponseInnerWeightLimits.from_json(json)
# print the JSON string representation of the object
print(ListCarrierProducts200ResponseInnerWeightLimits.to_json())

# convert the object into a dict
list_carrier_products200_response_inner_weight_limits_dict = list_carrier_products200_response_inner_weight_limits_instance.to_dict()
# create an instance of ListCarrierProducts200ResponseInnerWeightLimits from a dict
list_carrier_products200_response_inner_weight_limits_from_dict = ListCarrierProducts200ResponseInnerWeightLimits.from_dict(list_carrier_products200_response_inner_weight_limits_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


