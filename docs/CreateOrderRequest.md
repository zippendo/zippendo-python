# CreateOrderRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**order_number** | **str** | Human-readable order number. | 
**external_id** | **str** | Identifier of the order in the source platform. | [optional] 
**order_channel_id** | **str** | ID of the order channel this order belongs to. | 
**customer_name** | **str** | Customer full name. | [optional] 
**customer_email** | **str** | Customer email address. | [optional] 
**shipping_address** | [**CreateOrderRequestShippingAddress**](CreateOrderRequestShippingAddress.md) |  | [optional] 
**order_lines** | [**List[CreateOrderRequestOrderLinesInner]**](CreateOrderRequestOrderLinesInner.md) | Line items in the order. | 
**subtotal_amount** | **float** | Order subtotal before shipping and tax. | [optional] 
**total_amount** | **float** | Order grand total. | [optional] 
**currency** | **str** | ISO 4217 currency code. | [optional] 
**notes** | **str** | Free-form internal notes. | [optional] 
**shipping_rule_id** | **str** | Shipping rule to ship this order with. When set, a shipment is created immediately (and dispatched if the channel has autoShipOnCreate enabled). | [optional] 
**shipping_method_title** | **str** | Shipping-method title from the source checkout; matched against the order channel&#39;s shipping-method mappings to pick a shipping rule. | [optional] 
**external_data** | **Dict[str, object]** | Raw platform-specific payload for reference. | [optional] 

## Example

```python
from zippendo.models.create_order_request import CreateOrderRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateOrderRequest from a JSON string
create_order_request_instance = CreateOrderRequest.from_json(json)
# print the JSON string representation of the object
print(CreateOrderRequest.to_json())

# convert the object into a dict
create_order_request_dict = create_order_request_instance.to_dict()
# create an instance of CreateOrderRequest from a dict
create_order_request_from_dict = CreateOrderRequest.from_dict(create_order_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


