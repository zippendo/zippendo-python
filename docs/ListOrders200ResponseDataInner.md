# ListOrders200ResponseDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | Unique order ID. | 
**order_number** | **str** | Human-readable order number. | 
**customer_name** | **str** | Customer full name. | [optional] 
**customer_email** | **str** | Customer email address. | [optional] 
**status** | **str** | Order fulfilment status derived from its shipments. | 
**subtotal_amount** | **float** | Order subtotal before shipping and tax. | [optional] 
**total_amount** | **float** | Order grand total. | [optional] 
**currency** | **str** | ISO 4217 currency code. | [optional] 
**shipment_count** | **int** | Number of shipments created for the order. | 
**order_channel** | [**ListOrders200ResponseDataInnerOrderChannel**](ListOrders200ResponseDataInnerOrderChannel.md) |  | 
**created_at** | **str** | Creation timestamp (ISO 8601). | 
**updated_at** | **str** | Last update timestamp (ISO 8601). | 

## Example

```python
from zippendo.models.list_orders200_response_data_inner import ListOrders200ResponseDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of ListOrders200ResponseDataInner from a JSON string
list_orders200_response_data_inner_instance = ListOrders200ResponseDataInner.from_json(json)
# print the JSON string representation of the object
print(ListOrders200ResponseDataInner.to_json())

# convert the object into a dict
list_orders200_response_data_inner_dict = list_orders200_response_data_inner_instance.to_dict()
# create an instance of ListOrders200ResponseDataInner from a dict
list_orders200_response_data_inner_from_dict = ListOrders200ResponseDataInner.from_dict(list_orders200_response_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


