# RevokeOrderChannelWebhookSecret200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**revoked** | **bool** | Whether the signing secret was revoked. | 

## Example

```python
from zippendo.models.revoke_order_channel_webhook_secret200_response import RevokeOrderChannelWebhookSecret200Response

# TODO update the JSON string below
json = "{}"
# create an instance of RevokeOrderChannelWebhookSecret200Response from a JSON string
revoke_order_channel_webhook_secret200_response_instance = RevokeOrderChannelWebhookSecret200Response.from_json(json)
# print the JSON string representation of the object
print(RevokeOrderChannelWebhookSecret200Response.to_json())

# convert the object into a dict
revoke_order_channel_webhook_secret200_response_dict = revoke_order_channel_webhook_secret200_response_instance.to_dict()
# create an instance of RevokeOrderChannelWebhookSecret200Response from a dict
revoke_order_channel_webhook_secret200_response_from_dict = RevokeOrderChannelWebhookSecret200Response.from_dict(revoke_order_channel_webhook_secret200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


