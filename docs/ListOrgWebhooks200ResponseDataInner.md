# ListOrgWebhooks200ResponseDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | Webhook ID | 
**name** | **str** | Human-readable webhook name | 
**url** | **str** | Webhook endpoint URL | 
**events** | **List[str]** | Events the webhook is subscribed to | 
**is_active** | **bool** | Whether the webhook is active | 
**created_at** | **str** | Creation timestamp (ISO 8601) | 
**updated_at** | **str** | Last update timestamp (ISO 8601) | 

## Example

```python
from zippendo.models.list_org_webhooks200_response_data_inner import ListOrgWebhooks200ResponseDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of ListOrgWebhooks200ResponseDataInner from a JSON string
list_org_webhooks200_response_data_inner_instance = ListOrgWebhooks200ResponseDataInner.from_json(json)
# print the JSON string representation of the object
print(ListOrgWebhooks200ResponseDataInner.to_json())

# convert the object into a dict
list_org_webhooks200_response_data_inner_dict = list_org_webhooks200_response_data_inner_instance.to_dict()
# create an instance of ListOrgWebhooks200ResponseDataInner from a dict
list_org_webhooks200_response_data_inner_from_dict = ListOrgWebhooks200ResponseDataInner.from_dict(list_org_webhooks200_response_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


