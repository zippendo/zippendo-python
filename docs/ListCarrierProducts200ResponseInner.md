# ListCarrierProducts200ResponseInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** | Display name of the shipping product | 
**product_id** | **str** | Unique carrier product identifier | 
**type** | **str** | Direction of the shipment for this product | 
**description** | **str** | Description of the shipping product | [optional] 
**available_countries** | **List[str]** | Recipient countries supported by this product | 
**available_sender_countries** | **List[str]** | Sender countries supported by this product | 
**is_service_point** | **bool** | Whether delivery is to a service point/pickup location | [default to False]
**is_pickup_available** | **bool** | Whether carrier pickup is available for this product | [default to False]
**services** | [**List[ListCarrierProducts200ResponseInnerServicesInner]**](ListCarrierProducts200ResponseInnerServicesInner.md) | Additional services available for this product | [optional] 
**additional_parameters** | [**List[ListCarrierProducts200ResponseInnerAdditionalParametersInner]**](ListCarrierProducts200ResponseInnerAdditionalParametersInner.md) | Extra parameters that can or must be supplied for this product | [optional] 
**weight_limits** | [**ListCarrierProducts200ResponseInnerWeightLimits**](ListCarrierProducts200ResponseInnerWeightLimits.md) |  | [optional] 

## Example

```python
from zippendo.models.list_carrier_products200_response_inner import ListCarrierProducts200ResponseInner

# TODO update the JSON string below
json = "{}"
# create an instance of ListCarrierProducts200ResponseInner from a JSON string
list_carrier_products200_response_inner_instance = ListCarrierProducts200ResponseInner.from_json(json)
# print the JSON string representation of the object
print(ListCarrierProducts200ResponseInner.to_json())

# convert the object into a dict
list_carrier_products200_response_inner_dict = list_carrier_products200_response_inner_instance.to_dict()
# create an instance of ListCarrierProducts200ResponseInner from a dict
list_carrier_products200_response_inner_from_dict = ListCarrierProducts200ResponseInner.from_dict(list_carrier_products200_response_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


