# UpdateOrderRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**order_number** | **str** | Human-readable order number. | [optional] 
**customer_name** | **str** | Customer full name. | [optional] 
**customer_email** | **str** | Customer email address. | [optional] 
**shipping_address** | [**CreateOrderRequestShippingAddress**](CreateOrderRequestShippingAddress.md) |  | [optional] 
**order_lines** | [**List[CreateOrderRequestOrderLinesInner]**](CreateOrderRequestOrderLinesInner.md) | Line items in the order. | [optional] 
**subtotal_amount** | **float** | Order subtotal before shipping and tax. | [optional] 
**total_amount** | **float** | Order grand total. | [optional] 
**currency** | **str** | ISO 4217 currency code. | [optional] 
**notes** | **str** | Free-form internal notes. | [optional] 
**status** | **str** | Order fulfilment status derived from its shipments. | [optional] 
**shipping_rule_id** | **str** | ID of the shipping rule to apply. | [optional] 

## Example

```python
from zippendo.models.update_order_request import UpdateOrderRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateOrderRequest from a JSON string
update_order_request_instance = UpdateOrderRequest.from_json(json)
# print the JSON string representation of the object
print(UpdateOrderRequest.to_json())

# convert the object into a dict
update_order_request_dict = update_order_request_instance.to_dict()
# create an instance of UpdateOrderRequest from a dict
update_order_request_from_dict = UpdateOrderRequest.from_dict(update_order_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


