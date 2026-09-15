# UpdateOrderChannelRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**brand_id** | **str** | Brand this channel belongs to; null for organization-wide | [optional] 
**name** | **str** | Display name for the channel. | [optional] 
**enabled** | **bool** | Whether the channel is active. | [optional] 
**role** | **str** | What Zippendo is used for on this channel. &#x60;orders_and_rates&#x60; (default) imports orders and serves checkout rates. &#x60;rates_only&#x60; serves checkout rates and service-point selection ONLY — orders are owned by an external system such as a WMS, nothing is imported, and no fulfilment or tracking is pushed back to the platform. | [optional] 
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


