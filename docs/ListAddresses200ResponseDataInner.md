# ListAddresses200ResponseDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | Unique address identifier | 
**name** | **str** | Name of the address | 
**att_contact** | **str** | Attention contact person | 
**address1** | **str** | Address line 1 | 
**address2** | **str** | Address line 2 | 
**zipcode** | **str** | Postal/ZIP code | 
**city** | **str** | City | 
**phone** | **str** | Phone number | 
**country_code** | **str** | ISO country code | 
**state** | **str** | State/Province | 
**email** | **str** | Email address | 
**customs** | **Dict[str, str]** | Customs identifiers keyed by type | [optional] 
**address_types** | **List[str]** | Address types (sender, pickup, return) | 
**org_id** | **str** | Owning organization ID | 
**brand_id** | **str** | Brand this record belongs to, or null when it is organization-wide | 
**created_at** | **str** | Creation timestamp (ISO 8601) | 
**updated_at** | **str** | Last update timestamp (ISO 8601) | 

## Example

```python
from zippendo.models.list_addresses200_response_data_inner import ListAddresses200ResponseDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of ListAddresses200ResponseDataInner from a JSON string
list_addresses200_response_data_inner_instance = ListAddresses200ResponseDataInner.from_json(json)
# print the JSON string representation of the object
print(ListAddresses200ResponseDataInner.to_json())

# convert the object into a dict
list_addresses200_response_data_inner_dict = list_addresses200_response_data_inner_instance.to_dict()
# create an instance of ListAddresses200ResponseDataInner from a dict
list_addresses200_response_data_inner_from_dict = ListAddresses200ResponseDataInner.from_dict(list_addresses200_response_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


