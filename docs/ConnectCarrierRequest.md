# ConnectCarrierRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** | Carrier display name | 
**carrier_slug** | **str** | Carrier slug identifier | 
**config** | [**Dict[str, ListCarriers200ResponseDataInnerConfigValue]**](ListCarriers200ResponseDataInnerConfigValue.md) | Carrier configuration (required and optional fields) | 
**brand_id** | **str** | Brand this record is assigned to; null (or omitted outside a brand session) keeps it organization-wide | [optional] 

## Example

```python
from zippendo.models.connect_carrier_request import ConnectCarrierRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ConnectCarrierRequest from a JSON string
connect_carrier_request_instance = ConnectCarrierRequest.from_json(json)
# print the JSON string representation of the object
print(ConnectCarrierRequest.to_json())

# convert the object into a dict
connect_carrier_request_dict = connect_carrier_request_instance.to_dict()
# create an instance of ConnectCarrierRequest from a dict
connect_carrier_request_from_dict = ConnectCarrierRequest.from_dict(connect_carrier_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


