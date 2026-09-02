# GetOrderChannelWebhookStatus200ResponseWebhooksInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **float** | Platform webhook ID. | 
**topic** | **str** | Webhook event topic. | 
**address** | **str** | Registered callback address. | 
**created_at** | **str** | Webhook creation timestamp. | 
**delivery_url** | **str** | WooCommerce delivery URL (same as &#x60;address&#x60;; present for WooCommerce channels). | [optional] 
**status** | **str** | WooCommerce webhook status. A value other than &#x60;active&#x60; means WooCommerce disabled the webhook (e.g. after repeated delivery failures). | [optional] 

## Example

```python
from zippendo.models.get_order_channel_webhook_status200_response_webhooks_inner import GetOrderChannelWebhookStatus200ResponseWebhooksInner

# TODO update the JSON string below
json = "{}"
# create an instance of GetOrderChannelWebhookStatus200ResponseWebhooksInner from a JSON string
get_order_channel_webhook_status200_response_webhooks_inner_instance = GetOrderChannelWebhookStatus200ResponseWebhooksInner.from_json(json)
# print the JSON string representation of the object
print(GetOrderChannelWebhookStatus200ResponseWebhooksInner.to_json())

# convert the object into a dict
get_order_channel_webhook_status200_response_webhooks_inner_dict = get_order_channel_webhook_status200_response_webhooks_inner_instance.to_dict()
# create an instance of GetOrderChannelWebhookStatus200ResponseWebhooksInner from a dict
get_order_channel_webhook_status200_response_webhooks_inner_from_dict = GetOrderChannelWebhookStatus200ResponseWebhooksInner.from_dict(get_order_channel_webhook_status200_response_webhooks_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


