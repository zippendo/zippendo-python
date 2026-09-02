# UpdateOrderChannelRequestSettings

Partial channel settings to merge into existing settings. Server-managed fields (webhook secret/ids, checkout token) cannot be set here.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**use_webhooks** | **bool** | Use webhooks for real-time order sync. | [optional] [default to True]
**site_url** | **str** | WooCommerce store URL. | [optional] 
**auto_fulfill** | **bool** | Push tracking back to the platform when a shipment is dispatched. Enabled by default (opt-out) — set to false to disable write-back; an unset value still syncs. | [optional] 
**auto_sync** | **bool** | Periodically poll the channel for new orders. | [optional] [default to False]
**sync_interval_minutes** | **int** | Polling interval in minutes (5-1440). | [optional] [default to 15]
**auto_ship_on_create** | **bool** | Create a shipment automatically when an order arrives. | [optional] [default to False]
**default_carrier_id** | **str** | Default carrier ID for auto-shipping. | [optional] 
**default_product_id** | **str** | Default carrier product ID for auto-shipping. | [optional] 
**default_address_id** | **str** | Default sender address ID for auto-shipping. | [optional] 
**shipping_method_mappings** | [**List[CreateOrderChannelRequestSettingsShippingMethodMappingsInner]**](CreateOrderChannelRequestSettingsShippingMethodMappingsInner.md) | Map imported shipping-method titles to shipping rules, for channels without checkout rate integration. | [optional] 
**sync_only_unfulfilled** | **bool** | Only import orders that are not yet fulfilled. | [optional] [default to True]
**sync_orders_since** | **datetime** | Only sync orders placed at or after this timestamp. | [optional] 
**service_point_count** | **int** | Number of service points to show at checkout (1-20). | [optional] [default to 6]

## Example

```python
from zippendo.models.update_order_channel_request_settings import UpdateOrderChannelRequestSettings

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateOrderChannelRequestSettings from a JSON string
update_order_channel_request_settings_instance = UpdateOrderChannelRequestSettings.from_json(json)
# print the JSON string representation of the object
print(UpdateOrderChannelRequestSettings.to_json())

# convert the object into a dict
update_order_channel_request_settings_dict = update_order_channel_request_settings_instance.to_dict()
# create an instance of UpdateOrderChannelRequestSettings from a dict
update_order_channel_request_settings_from_dict = UpdateOrderChannelRequestSettings.from_dict(update_order_channel_request_settings_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


