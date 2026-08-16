# CreateOrgWebhookRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** | Human-readable webhook name | 
**url** | **str** | Webhook endpoint URL | 
**events** | **List[str]** | Events to subscribe to | 
**is_active** | **bool** | Whether the webhook is active | [optional] [default to True]
**brand_id** | **str** | Brand this record is assigned to; null (or omitted outside a brand session) keeps it organization-wide | [optional] 

## Example

```python
from zippendo.models.create_org_webhook_request import CreateOrgWebhookRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateOrgWebhookRequest from a JSON string
create_org_webhook_request_instance = CreateOrgWebhookRequest.from_json(json)
# print the JSON string representation of the object
print(CreateOrgWebhookRequest.to_json())

# convert the object into a dict
create_org_webhook_request_dict = create_org_webhook_request_instance.to_dict()
# create an instance of CreateOrgWebhookRequest from a dict
create_org_webhook_request_from_dict = CreateOrgWebhookRequest.from_dict(create_org_webhook_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


