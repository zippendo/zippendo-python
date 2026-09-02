# UpdateOrderChannelRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**brand_id** | **str** | Brand this channel belongs to; null for organization-wide | [optional] 
**name** | **str** | Display name for the channel. | [optional] 
**enabled** | **bool** | Whether the channel is active. | [optional] 
**credentials** | **Dict[str, object]** | Type-specific platform credentials. | [optional] 
**settings** | [**UpdateOrderChannelRequestSettings**](UpdateOrderChannelRequestSettings.md) |  | [optional] 
**shipping_rule_ids** | **List[str]** | IDs of shipping rules linked to this channel. | [optional] 

## Example

```python
from zippendo.models.update_order_channel_request import UpdateOrderChannelRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateOrderChannelRequest from a JSON string
update_order_channel_request_instance = UpdateOrderChannelRequest.from_json(json)
# print the JSON string representation of the object
print(UpdateOrderChannelRequest.to_json())

# convert the object into a dict
update_order_channel_request_dict = update_order_channel_request_instance.to_dict()
# create an instance of UpdateOrderChannelRequest from a dict
update_order_channel_request_from_dict = UpdateOrderChannelRequest.from_dict(update_order_channel_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


