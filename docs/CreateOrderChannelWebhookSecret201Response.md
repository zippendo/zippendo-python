# CreateOrderChannelWebhookSecret201Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**secret** | **str** | The webhook signing secret. Returned only once — store it in your system; every push to the ingest URL must carry an HMAC-SHA256 hex signature of the raw body computed with it. | 
**webhook_url** | **str** | The ingest URL your system pushes signed order events to. | 
**created_at** | **datetime** | When this secret was issued (ISO 8601). | 

## Example

```python
from zippendo.models.create_order_channel_webhook_secret201_response import CreateOrderChannelWebhookSecret201Response

# TODO update the JSON string below
json = "{}"
# create an instance of CreateOrderChannelWebhookSecret201Response from a JSON string
create_order_channel_webhook_secret201_response_instance = CreateOrderChannelWebhookSecret201Response.from_json(json)
# print the JSON string representation of the object
print(CreateOrderChannelWebhookSecret201Response.to_json())

# convert the object into a dict
create_order_channel_webhook_secret201_response_dict = create_order_channel_webhook_secret201_response_instance.to_dict()
# create an instance of CreateOrderChannelWebhookSecret201Response from a dict
create_order_channel_webhook_secret201_response_from_dict = CreateOrderChannelWebhookSecret201Response.from_dict(create_order_channel_webhook_secret201_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


