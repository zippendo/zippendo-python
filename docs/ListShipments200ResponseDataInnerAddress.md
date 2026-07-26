# ListShipments200ResponseDataInnerAddress


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
**created_at** | **str** | Creation timestamp (ISO 8601) | 
**updated_at** | **str** | Last update timestamp (ISO 8601) | 

## Example

```python
from zippendo.models.list_shipments200_response_data_inner_address import ListShipments200ResponseDataInnerAddress

# TODO update the JSON string below
json = "{}"
# create an instance of ListShipments200ResponseDataInnerAddress from a JSON string
list_shipments200_response_data_inner_address_instance = ListShipments200ResponseDataInnerAddress.from_json(json)
# print the JSON string representation of the object
print(ListShipments200ResponseDataInnerAddress.to_json())

# convert the object into a dict
list_shipments200_response_data_inner_address_dict = list_shipments200_response_data_inner_address_instance.to_dict()
# create an instance of ListShipments200ResponseDataInnerAddress from a dict
list_shipments200_response_data_inner_address_from_dict = ListShipments200ResponseDataInnerAddress.from_dict(list_shipments200_response_data_inner_address_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


