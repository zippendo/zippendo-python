# GetOrder200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | Unique order ID. | 
**order_number** | **str** | Human-readable order number. | 
**external_id** | **str** | Identifier of the order in the source platform. | [optional] 
**customer_name** | **str** | Customer full name. | [optional] 
**customer_email** | **str** | Customer email address. | [optional] 
**shipping_address** | [**CreateOrder201ResponseShippingAddress**](CreateOrder201ResponseShippingAddress.md) |  | [optional] 
**order_lines** | [**List[CreateOrder201ResponseOrderLinesInner]**](CreateOrder201ResponseOrderLinesInner.md) | Line items in the order. | 
**subtotal_amount** | **float** | Order subtotal before shipping and tax. | [optional] 
**total_amount** | **float** | Order grand total. | [optional] 
**currency** | **str** | ISO 4217 currency code. | [optional] 
**status** | **str** | Order fulfilment status derived from its shipments. | 
**shipping_rule_id** | **str** | ID of the applied shipping rule. | [optional] 
**notes** | **str** | Free-form internal notes. | [optional] 
**external_data** | **Dict[str, object]** | Raw platform-specific payload for reference. | [optional] 
**order_channel_id** | **str** | ID of the order channel this order belongs to. | 
**org_id** | **str** | Owning organization ID. | 
**created_at** | **str** | Creation timestamp (ISO 8601). | 
**updated_at** | **str** | Last update timestamp (ISO 8601). | 
**order_channel** | [**ListOrders200ResponseDataInnerOrderChannel**](ListOrders200ResponseDataInnerOrderChannel.md) |  | 
**shipping_rule** | [**GetOrder200ResponseShippingRule**](GetOrder200ResponseShippingRule.md) |  | [optional] 
**shipments** | [**List[GetOrder200ResponseShipmentsInner]**](GetOrder200ResponseShipmentsInner.md) |  | 

## Example

```python
from zippendo.models.get_order200_response import GetOrder200Response

# TODO update the JSON string below
json = "{}"
# create an instance of GetOrder200Response from a JSON string
get_order200_response_instance = GetOrder200Response.from_json(json)
# print the JSON string representation of the object
print(GetOrder200Response.to_json())

# convert the object into a dict
get_order200_response_dict = get_order200_response_instance.to_dict()
# create an instance of GetOrder200Response from a dict
get_order200_response_from_dict = GetOrder200Response.from_dict(get_order200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


