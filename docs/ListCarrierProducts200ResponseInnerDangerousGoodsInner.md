# ListCarrierProducts200ResponseInnerDangerousGoodsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**kind** | **str** | &#x60;limited_quantity&#x60;: dangerous goods packed in limited quantities (LQ). &#x60;regulated&#x60;: fully regulated dangerous goods (ADR). | 
**service_id** | **str** | The service that declares these dangerous goods to the carrier. | 
**parameters** | [**ListCarrierProducts200ResponseInnerDangerousGoodsInnerParameters**](ListCarrierProducts200ResponseInnerDangerousGoodsInnerParameters.md) |  | 
**owned_parameters** | **List[str]** | Every additional parameter that describes the declared goods, including those &#x60;parameters&#x60; does not fill. A declaration replaces them all, so a value saved for other goods is never sent. | [optional] 
**single_parcel** | **bool** | The carrier takes this declaration on a shipment of one parcel only. | [optional] 

## Example

```python
from zippendo.models.list_carrier_products200_response_inner_dangerous_goods_inner import ListCarrierProducts200ResponseInnerDangerousGoodsInner

# TODO update the JSON string below
json = "{}"
# create an instance of ListCarrierProducts200ResponseInnerDangerousGoodsInner from a JSON string
list_carrier_products200_response_inner_dangerous_goods_inner_instance = ListCarrierProducts200ResponseInnerDangerousGoodsInner.from_json(json)
# print the JSON string representation of the object
print(ListCarrierProducts200ResponseInnerDangerousGoodsInner.to_json())

# convert the object into a dict
list_carrier_products200_response_inner_dangerous_goods_inner_dict = list_carrier_products200_response_inner_dangerous_goods_inner_instance.to_dict()
# create an instance of ListCarrierProducts200ResponseInnerDangerousGoodsInner from a dict
list_carrier_products200_response_inner_dangerous_goods_inner_from_dict = ListCarrierProducts200ResponseInnerDangerousGoodsInner.from_dict(list_carrier_products200_response_inner_dangerous_goods_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


