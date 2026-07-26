# ListOrders200ResponseDataInnerOrderChannel

Summary of the order's source channel.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | Order channel ID. | 
**name** | **str** | Order channel name. | 
**type** | **str** | Type of the order channel (sales platform). | 

## Example

```python
from zippendo.models.list_orders200_response_data_inner_order_channel import ListOrders200ResponseDataInnerOrderChannel

# TODO update the JSON string below
json = "{}"
# create an instance of ListOrders200ResponseDataInnerOrderChannel from a JSON string
list_orders200_response_data_inner_order_channel_instance = ListOrders200ResponseDataInnerOrderChannel.from_json(json)
# print the JSON string representation of the object
print(ListOrders200ResponseDataInnerOrderChannel.to_json())

# convert the object into a dict
list_orders200_response_data_inner_order_channel_dict = list_orders200_response_data_inner_order_channel_instance.to_dict()
# create an instance of ListOrders200ResponseDataInnerOrderChannel from a dict
list_orders200_response_data_inner_order_channel_from_dict = ListOrders200ResponseDataInnerOrderChannel.from_dict(list_orders200_response_data_inner_order_channel_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


