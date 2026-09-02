# ListOrderChannels200ResponseDataInnerSettings

Channel settings (webhook secret and checkout token hash omitted).

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**use_webhooks** | **bool** | Use webhooks for real-time order sync. | [default to True]
**webhook_id** | **str** | External webhook identifier for management. | [optional] 
**webhook_ids** | **List[int]** | Registered WooCommerce webhook ids. | [optional] 
**webhook_secret_created_at** | **datetime** | When the custom channel&#39;s webhook signing secret was issued. A non-secret signal so clients can show that a secret exists; the secret itself is never returned after creation. | [optional] 
**site_url** | **str** | WooCommerce store URL. | [optional] 
**auto_fulfill** | **bool** | Push tracking back to the platform when a shipment is dispatched. Enabled by default (opt-out) — set to false to disable write-back; an unset value still syncs. | [optional] 
**checkout_token_created_at** | **datetime** | When the checkout token was issued (internal; never exposed in API responses). | [optional] 
**auto_sync** | **bool** | Periodically poll the channel for new orders. | [default to False]
**sync_interval_minutes** | **int** | Polling interval in minutes (5-1440). | [default to 15]
**auto_ship_on_create** | **bool** | Create a shipment automatically when an order arrives. | [default to False]
**default_carrier_id** | **str** | Default carrier ID for auto-shipping. | [optional] 
**default_product_id** | **str** | Default carrier product ID for auto-shipping. | [optional] 
**default_address_id** | **str** | Default sender address ID for auto-shipping. | [optional] 
**shipping_method_mappings** | [**List[ListOrderChannels200ResponseDataInnerSettingsShippingMethodMappingsInner]**](ListOrderChannels200ResponseDataInnerSettingsShippingMethodMappingsInner.md) | Map imported shipping-method titles to shipping rules, for channels without checkout rate integration. | [optional] 
**sync_only_unfulfilled** | **bool** | Only import orders that are not yet fulfilled. | [default to True]
**sync_orders_since** | **datetime** | Only sync orders placed at or after this timestamp. | [optional] 
**service_point_count** | **int** | Number of service points to show at checkout (1-20). | [default to 6]

## Example

```python
from zippendo.models.list_order_channels200_response_data_inner_settings import ListOrderChannels200ResponseDataInnerSettings

# TODO update the JSON string below
json = "{}"
# create an instance of ListOrderChannels200ResponseDataInnerSettings from a JSON string
list_order_channels200_response_data_inner_settings_instance = ListOrderChannels200ResponseDataInnerSettings.from_json(json)
# print the JSON string representation of the object
print(ListOrderChannels200ResponseDataInnerSettings.to_json())

# convert the object into a dict
list_order_channels200_response_data_inner_settings_dict = list_order_channels200_response_data_inner_settings_instance.to_dict()
# create an instance of ListOrderChannels200ResponseDataInnerSettings from a dict
list_order_channels200_response_data_inner_settings_from_dict = ListOrderChannels200ResponseDataInnerSettings.from_dict(list_order_channels200_response_data_inner_settings_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


