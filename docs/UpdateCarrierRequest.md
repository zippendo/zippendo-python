# UpdateCarrierRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** | Carrier display name | [optional] 
**carrier_slug** | **str** | Carrier slug identifier | [optional] 
**config** | [**Dict[str, ListCarriers200ResponseDataInnerConfigValue]**](ListCarriers200ResponseDataInnerConfigValue.md) | Carrier configuration (required and optional fields) | [optional] 

## Example

```python
from zippendo.models.update_carrier_request import UpdateCarrierRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateCarrierRequest from a JSON string
update_carrier_request_instance = UpdateCarrierRequest.from_json(json)
# print the JSON string representation of the object
print(UpdateCarrierRequest.to_json())

# convert the object into a dict
update_carrier_request_dict = update_carrier_request_instance.to_dict()
# create an instance of UpdateCarrierRequest from a dict
update_carrier_request_from_dict = UpdateCarrierRequest.from_dict(update_carrier_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


