# ListCarriers200ResponseDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | Unique carrier identifier | 
**name** | **str** | Carrier display name | 
**carrier_slug** | **str** | Carrier slug identifier | 
**config** | [**Dict[str, ListCarriers200ResponseDataInnerConfigValue]**](ListCarriers200ResponseDataInnerConfigValue.md) | Carrier configuration (required and optional fields) | 
**org_id** | **str** | Owning organization ID | 
**brand_id** | **str** | Brand this record belongs to, or null when it is organization-wide | 
**created_at** | **str** | Creation timestamp (ISO 8601) | 
**updated_at** | **str** | Last update timestamp (ISO 8601) | 
**logo** | **str** | Carrier logo URL | [optional] 
**brand_color** | **str** | Carrier brand color (hex) | [optional] 
**deprecated** | **bool** | Whether this carrier integration is deprecated (still works, but discouraged) | [optional] 
**deprecation_message** | **str** | Guidance shown alongside the deprecated tag (e.g. what to migrate to) | [optional] 
**generates_customs_documents** | **bool** | Whether the carrier produces the customs declaration (CN22/CN23) itself and returns it with the label. | [optional] 
**generates_commercial_invoice** | **bool** | Whether the carrier produces the commercial invoice itself and returns it with the label, e.g. via electronic trade documents. | [optional] 

## Example

```python
from zippendo.models.list_carriers200_response_data_inner import ListCarriers200ResponseDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of ListCarriers200ResponseDataInner from a JSON string
list_carriers200_response_data_inner_instance = ListCarriers200ResponseDataInner.from_json(json)
# print the JSON string representation of the object
print(ListCarriers200ResponseDataInner.to_json())

# convert the object into a dict
list_carriers200_response_data_inner_dict = list_carriers200_response_data_inner_instance.to_dict()
# create an instance of ListCarriers200ResponseDataInner from a dict
list_carriers200_response_data_inner_from_dict = ListCarriers200ResponseDataInner.from_dict(list_carriers200_response_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


