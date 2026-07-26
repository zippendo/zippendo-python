# CreateOrgWebhook201Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | Webhook ID | 
**name** | **str** | Human-readable webhook name | 
**url** | **str** | Webhook endpoint URL | 
**secret** | **str** | Signing secret used to verify webhook payloads | 
**events** | **List[str]** | Events the webhook is subscribed to | 
**is_active** | **bool** | Whether the webhook is active | 
**created_at** | **str** | Creation timestamp (ISO 8601) | 
**updated_at** | **str** | Last update timestamp (ISO 8601) | 

## Example

```python
from zippendo.models.create_org_webhook201_response import CreateOrgWebhook201Response

# TODO update the JSON string below
json = "{}"
# create an instance of CreateOrgWebhook201Response from a JSON string
create_org_webhook201_response_instance = CreateOrgWebhook201Response.from_json(json)
# print the JSON string representation of the object
print(CreateOrgWebhook201Response.to_json())

# convert the object into a dict
create_org_webhook201_response_dict = create_org_webhook201_response_instance.to_dict()
# create an instance of CreateOrgWebhook201Response from a dict
create_org_webhook201_response_from_dict = CreateOrgWebhook201Response.from_dict(create_org_webhook201_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


