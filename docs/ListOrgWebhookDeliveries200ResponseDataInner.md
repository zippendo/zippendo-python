# ListOrgWebhookDeliveries200ResponseDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | Delivery log ID | 
**webhook_id** | **str** | ID of the webhook this delivery belongs to | 
**event** | **str** | Event type that was delivered | 
**payload** | **object** | JSON payload that was sent | 
**status_code** | **float** | HTTP status code returned by the endpoint | 
**response** | **str** | Response body returned by the endpoint | 
**duration** | **float** | Request duration in milliseconds | 
**success** | **bool** | Whether the delivery succeeded | 
**attempt** | **float** | Delivery attempt number | 
**error** | **str** | Error message if the delivery failed | 
**created_at** | **str** | Delivery timestamp (ISO 8601) | 

## Example

```python
from zippendo.models.list_org_webhook_deliveries200_response_data_inner import ListOrgWebhookDeliveries200ResponseDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of ListOrgWebhookDeliveries200ResponseDataInner from a JSON string
list_org_webhook_deliveries200_response_data_inner_instance = ListOrgWebhookDeliveries200ResponseDataInner.from_json(json)
# print the JSON string representation of the object
print(ListOrgWebhookDeliveries200ResponseDataInner.to_json())

# convert the object into a dict
list_org_webhook_deliveries200_response_data_inner_dict = list_org_webhook_deliveries200_response_data_inner_instance.to_dict()
# create an instance of ListOrgWebhookDeliveries200ResponseDataInner from a dict
list_org_webhook_deliveries200_response_data_inner_from_dict = ListOrgWebhookDeliveries200ResponseDataInner.from_dict(list_org_webhook_deliveries200_response_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


