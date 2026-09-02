# CreateOrderChannelRequestSettingsShippingMethodMappingsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**match** | **str** | Shipping-method title to match against imported orders (trimmed, case-insensitive, exact). | 
**shipping_rule_id** | **str** | Shipping rule applied to orders whose shipping-method title matches. | 
**service_point_selection** | **str** | For rules whose product delivers to a service point: &#39;nearest&#39; auto-selects the closest point to the recipient address; &#39;manual&#39; keeps the shipment in draft for manual selection. | [optional] 

## Example

```python
from zippendo.models.create_order_channel_request_settings_shipping_method_mappings_inner import CreateOrderChannelRequestSettingsShippingMethodMappingsInner

# TODO update the JSON string below
json = "{}"
# create an instance of CreateOrderChannelRequestSettingsShippingMethodMappingsInner from a JSON string
create_order_channel_request_settings_shipping_method_mappings_inner_instance = CreateOrderChannelRequestSettingsShippingMethodMappingsInner.from_json(json)
# print the JSON string representation of the object
print(CreateOrderChannelRequestSettingsShippingMethodMappingsInner.to_json())

# convert the object into a dict
create_order_channel_request_settings_shipping_method_mappings_inner_dict = create_order_channel_request_settings_shipping_method_mappings_inner_instance.to_dict()
# create an instance of CreateOrderChannelRequestSettingsShippingMethodMappingsInner from a dict
create_order_channel_request_settings_shipping_method_mappings_inner_from_dict = CreateOrderChannelRequestSettingsShippingMethodMappingsInner.from_dict(create_order_channel_request_settings_shipping_method_mappings_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


