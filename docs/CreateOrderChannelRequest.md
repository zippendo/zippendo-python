# CreateOrderChannelRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** | Display name for the channel. | 
**type** | **str** | Type of the order channel. Platform channels (Shopify, WooCommerce) are created via their connect flows. | 
**brand_id** | **str** | Brand this channel belongs to; null for organization-wide | [optional] 
**enabled** | **bool** | Whether the channel is active. | [optional] [default to True]
**settings** | [**CreateOrderChannelRequestSettings**](CreateOrderChannelRequestSettings.md) |  | [optional] 

## Example

```python
from zippendo.models.create_order_channel_request import CreateOrderChannelRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateOrderChannelRequest from a JSON string
create_order_channel_request_instance = CreateOrderChannelRequest.from_json(json)
# print the JSON string representation of the object
print(CreateOrderChannelRequest.to_json())

# convert the object into a dict
create_order_channel_request_dict = create_order_channel_request_instance.to_dict()
# create an instance of CreateOrderChannelRequest from a dict
create_order_channel_request_from_dict = CreateOrderChannelRequest.from_dict(create_order_channel_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


