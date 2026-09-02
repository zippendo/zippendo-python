# GetOrderChannelWebhookStatus200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**enabled** | **bool** | Whether webhooks are enabled for the channel. | 
**webhook_url** | **str** | Expected callback URL for this channel. | 
**webhooks** | [**List[GetOrderChannelWebhookStatus200ResponseWebhooksInner]**](GetOrderChannelWebhookStatus200ResponseWebhooksInner.md) | Webhooks registered for this channel&#39;s callback URL. | 

## Example

```python
from zippendo.models.get_order_channel_webhook_status200_response import GetOrderChannelWebhookStatus200Response

# TODO update the JSON string below
json = "{}"
# create an instance of GetOrderChannelWebhookStatus200Response from a JSON string
get_order_channel_webhook_status200_response_instance = GetOrderChannelWebhookStatus200Response.from_json(json)
# print the JSON string representation of the object
print(GetOrderChannelWebhookStatus200Response.to_json())

# convert the object into a dict
get_order_channel_webhook_status200_response_dict = get_order_channel_webhook_status200_response_instance.to_dict()
# create an instance of GetOrderChannelWebhookStatus200Response from a dict
get_order_channel_webhook_status200_response_from_dict = GetOrderChannelWebhookStatus200Response.from_dict(get_order_channel_webhook_status200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


