# UpdateOrgWebhookRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** | Human-readable webhook name | [optional] 
**url** | **str** | Webhook endpoint URL | [optional] 
**events** | **List[str]** | Events to subscribe to | [optional] 
**is_active** | **bool** | Whether the webhook is active | [optional] 

## Example

```python
from zippendo.models.update_org_webhook_request import UpdateOrgWebhookRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateOrgWebhookRequest from a JSON string
update_org_webhook_request_instance = UpdateOrgWebhookRequest.from_json(json)
# print the JSON string representation of the object
print(UpdateOrgWebhookRequest.to_json())

# convert the object into a dict
update_org_webhook_request_dict = update_org_webhook_request_instance.to_dict()
# create an instance of UpdateOrgWebhookRequest from a dict
update_org_webhook_request_from_dict = UpdateOrgWebhookRequest.from_dict(update_org_webhook_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


