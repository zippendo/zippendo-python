# UpdateAddressRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** | Name of the address | [optional] 
**att_contact** | **str** | Attention contact person | [optional] 
**address1** | **str** | Address line 1 | [optional] 
**address2** | **str** | Address line 2 | [optional] 
**zipcode** | **str** | Postal/ZIP code | [optional] 
**city** | **str** | City | [optional] 
**phone** | **str** | Phone number | [optional] 
**country_code** | **str** | ISO country code | [optional] 
**state** | **str** | State/Province | [optional] 
**email** | **str** | Email address | [optional] 
**customs** | **Dict[str, str]** | Customs identifiers | [optional] 
**address_types** | **List[str]** | Address types (sender, pickup, return) | [optional] 
**brand_id** | **str** | Brand this record is assigned to; null (or omitted outside a brand session) keeps it organization-wide | [optional] 

## Example

```python
from zippendo.models.update_address_request import UpdateAddressRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateAddressRequest from a JSON string
update_address_request_instance = UpdateAddressRequest.from_json(json)
# print the JSON string representation of the object
print(UpdateAddressRequest.to_json())

# convert the object into a dict
update_address_request_dict = update_address_request_instance.to_dict()
# create an instance of UpdateAddressRequest from a dict
update_address_request_from_dict = UpdateAddressRequest.from_dict(update_address_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


