# ListCarrierProductServicePoints200ResponseInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**lat** | **float** | Latitude of the service point | 
**lng** | **float** | Longitude of the service point | 
**name** | **str** | Name of the service point | 
**service_point_id** | **str** | Unique service point identifier | 
**opening_hours** | **List[str]** | Opening hours of the service point | [optional] 
**description** | **str** | Additional description of the service point | [optional] 
**distance** | **float** | Distance from the searched location in meters | [optional] 
**address** | [**ListCarrierProductServicePoints200ResponseInnerAddress**](ListCarrierProductServicePoints200ResponseInnerAddress.md) |  | [optional] 

## Example

```python
from zippendo.models.list_carrier_product_service_points200_response_inner import ListCarrierProductServicePoints200ResponseInner

# TODO update the JSON string below
json = "{}"
# create an instance of ListCarrierProductServicePoints200ResponseInner from a JSON string
list_carrier_product_service_points200_response_inner_instance = ListCarrierProductServicePoints200ResponseInner.from_json(json)
# print the JSON string representation of the object
print(ListCarrierProductServicePoints200ResponseInner.to_json())

# convert the object into a dict
list_carrier_product_service_points200_response_inner_dict = list_carrier_product_service_points200_response_inner_instance.to_dict()
# create an instance of ListCarrierProductServicePoints200ResponseInner from a dict
list_carrier_product_service_points200_response_inner_from_dict = ListCarrierProductServicePoints200ResponseInner.from_dict(list_carrier_product_service_points200_response_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


