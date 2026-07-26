# ListShippingRules200ResponseDataInnerCarrier


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | Unique carrier identifier | 
**name** | **str** | Carrier display name | 
**carrier_slug** | **str** | Carrier slug identifier | 
**config** | [**Dict[str, ListCarriers200ResponseDataInnerConfigValue]**](ListCarriers200ResponseDataInnerConfigValue.md) | Carrier configuration (required and optional fields) | 
**org_id** | **str** | Owning organization ID | 
**created_at** | **str** | Creation timestamp (ISO 8601) | 
**updated_at** | **str** | Last update timestamp (ISO 8601) | 

## Example

```python
from zippendo.models.list_shipping_rules200_response_data_inner_carrier import ListShippingRules200ResponseDataInnerCarrier

# TODO update the JSON string below
json = "{}"
# create an instance of ListShippingRules200ResponseDataInnerCarrier from a JSON string
list_shipping_rules200_response_data_inner_carrier_instance = ListShippingRules200ResponseDataInnerCarrier.from_json(json)
# print the JSON string representation of the object
print(ListShippingRules200ResponseDataInnerCarrier.to_json())

# convert the object into a dict
list_shipping_rules200_response_data_inner_carrier_dict = list_shipping_rules200_response_data_inner_carrier_instance.to_dict()
# create an instance of ListShippingRules200ResponseDataInnerCarrier from a dict
list_shipping_rules200_response_data_inner_carrier_from_dict = ListShippingRules200ResponseDataInnerCarrier.from_dict(list_shipping_rules200_response_data_inner_carrier_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


