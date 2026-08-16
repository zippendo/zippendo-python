# CreateAddressRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** | Name of the address | 
**att_contact** | **str** | Attention contact person | 
**address1** | **str** | Address line 1 | 
**address2** | **str** | Address line 2 | [optional] 
**zipcode** | **str** | Postal/ZIP code | 
**city** | **str** | City | 
**phone** | **str** | Phone number | 
**country_code** | **str** | Country code (ISO 2 or 3 letter) | 
**state** | **str** | State/Province | [optional] 
**email** | **str** | Email address | 
**customs** | **Dict[str, str]** | Customs identifiers (voec, eori, sprn, ioss, fda, duns) | [optional] 
**address_types** | **List[str]** | Address types (sender, pickup, return) | [optional] [default to ["sender"]]
**brand_id** | **str** | Brand this record is assigned to; null (or omitted outside a brand session) keeps it organization-wide | [optional] 

## Example

```python
from zippendo.models.create_address_request import CreateAddressRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateAddressRequest from a JSON string
create_address_request_instance = CreateAddressRequest.from_json(json)
# print the JSON string representation of the object
print(CreateAddressRequest.to_json())

# convert the object into a dict
create_address_request_dict = create_address_request_instance.to_dict()
# create an instance of CreateAddressRequest from a dict
create_address_request_from_dict = CreateAddressRequest.from_dict(create_address_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


