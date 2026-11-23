# ListCarrierProducts200ResponseInnerDangerousGoodsInnerParameters

Which additional parameters carry the details of the goods. Absent ones are not sent.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**un_number** | **str** | Key of the additional parameter that takes the four-digit UN number. | [optional] 
**hazard_class** | **str** | Key of the additional parameter that takes the ADR hazard class. | [optional] 
**packing_group** | **str** | Key of the additional parameter that takes the packing group (I, II or III). | [optional] 
**proper_shipping_name** | **str** | Key of the additional parameter that takes the proper shipping name. | [optional] 
**weight_grams_per_parcel** | **str** | Key of the additional parameter that takes the weight of the dangerous goods in the heaviest parcel, in grams. | [optional] 
**weight_kg** | **str** | Key of the additional parameter that takes the total weight of the dangerous goods, in kg. | [optional] 
**weight_kg_per_parcel** | **str** | Key of the additional parameter that takes the weight of the dangerous goods in the heaviest parcel, in kg. | [optional] 

## Example

```python
from zippendo.models.list_carrier_products200_response_inner_dangerous_goods_inner_parameters import ListCarrierProducts200ResponseInnerDangerousGoodsInnerParameters

# TODO update the JSON string below
json = "{}"
# create an instance of ListCarrierProducts200ResponseInnerDangerousGoodsInnerParameters from a JSON string
list_carrier_products200_response_inner_dangerous_goods_inner_parameters_instance = ListCarrierProducts200ResponseInnerDangerousGoodsInnerParameters.from_json(json)
# print the JSON string representation of the object
print(ListCarrierProducts200ResponseInnerDangerousGoodsInnerParameters.to_json())

# convert the object into a dict
list_carrier_products200_response_inner_dangerous_goods_inner_parameters_dict = list_carrier_products200_response_inner_dangerous_goods_inner_parameters_instance.to_dict()
# create an instance of ListCarrierProducts200ResponseInnerDangerousGoodsInnerParameters from a dict
list_carrier_products200_response_inner_dangerous_goods_inner_parameters_from_dict = ListCarrierProducts200ResponseInnerDangerousGoodsInnerParameters.from_dict(list_carrier_products200_response_inner_dangerous_goods_inner_parameters_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


