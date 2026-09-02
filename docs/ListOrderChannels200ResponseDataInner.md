# ListOrderChannels200ResponseDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | Unique order channel ID. | 
**name** | **str** | Display name of the channel. | 
**type** | **str** | Type of the order channel (sales platform). | 
**enabled** | **bool** | Whether the channel is active. | 
**brand_id** | **str** | Brand this channel belongs to, or null for organization-wide. Orders synced from this channel inherit it, and so do the shipments and documents made from them. | 
**has_credentials** | **bool** | Whether credentials are configured (values are never exposed). | 
**settings** | [**ListOrderChannels200ResponseDataInnerSettings**](ListOrderChannels200ResponseDataInnerSettings.md) |  | 
**webhooks_enabled** | **bool** | Whether real-time webhooks are enabled. | [optional] 
**last_sync_at** | **datetime** | Timestamp of the last successful sync. | [optional] 
**last_sync_error** | **str** | Error message from the last failed sync. | [optional] 
**shipping_rule_ids** | **List[str]** | IDs of shipping rules linked to this channel. | [optional] 
**org_id** | **str** | Owning organization ID. | 
**created_at** | **str** | Creation timestamp (ISO 8601). | 
**updated_at** | **str** | Last update timestamp (ISO 8601). | 

## Example

```python
from zippendo.models.list_order_channels200_response_data_inner import ListOrderChannels200ResponseDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of ListOrderChannels200ResponseDataInner from a JSON string
list_order_channels200_response_data_inner_instance = ListOrderChannels200ResponseDataInner.from_json(json)
# print the JSON string representation of the object
print(ListOrderChannels200ResponseDataInner.to_json())

# convert the object into a dict
list_order_channels200_response_data_inner_dict = list_order_channels200_response_data_inner_instance.to_dict()
# create an instance of ListOrderChannels200ResponseDataInner from a dict
list_order_channels200_response_data_inner_from_dict = ListOrderChannels200ResponseDataInner.from_dict(list_order_channels200_response_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


