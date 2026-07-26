# CreateOrder201Response


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

## Example

```python
from zippendo.models.create_order201_response import CreateOrder201Response

# TODO update the JSON string below
json = "{}"
# create an instance of CreateOrder201Response from a JSON string
create_order201_response_instance = CreateOrder201Response.from_json(json)
# print the JSON string representation of the object
print(CreateOrder201Response.to_json())

# convert the object into a dict
create_order201_response_dict = create_order201_response_instance.to_dict()
# create an instance of CreateOrder201Response from a dict
create_order201_response_from_dict = CreateOrder201Response.from_dict(create_order201_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


