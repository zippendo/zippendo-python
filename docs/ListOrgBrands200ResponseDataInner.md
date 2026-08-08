# ListOrgBrands200ResponseDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**company_name** | **str** | Legal entity name printed on this brand&#39;s documents | [optional] 
**vat_number** | **str** | VAT/tax ID for this brand&#39;s shipments and documents | [optional] 
**customs** | **Dict[str, str]** | Customs identifiers keyed by type | [optional] 
**address_line1** | **str** | Street address line 1 | [optional] 
**address_line2** | **str** | Street address line 2 | [optional] 
**city** | **str** | City | [optional] 
**postal_code** | **str** | Postal code | [optional] 
**country** | **str** | Country (ISO 3166-1 alpha-2) | [optional] 
**primary_color** | **str** | Primary brand colour — document title and table headers | [optional] 
**secondary_color** | **str** | Secondary brand colour — subtitle, section headings, totals accent | [optional] 
**id** | **str** | Unique brand identifier | 
**org_id** | **str** | Owning organization | 
**name** | **str** | Brand display name | 
**slug** | **str** | URL-safe identifier, unique within the organization | 
**use_org_customs** | **bool** | Whether this brand ships under the organization&#39;s fiscal identity. True (the default) declares the organization&#39;s VAT number and customs identifiers and ignores the brand&#39;s own. False makes the brand&#39;s own values the sole source — nothing falls back to the organization, so an identifier the brand has not set is not declared at all. | 
**logo_url** | **str** | Authenticated URL for the brand logo, or null when none is set | 
**archived_at** | **str** | When the brand was archived; null when active | 
**created_at** | **str** | Creation timestamp (ISO 8601) | 
**updated_at** | **str** | Last update timestamp (ISO 8601) | 

## Example

```python
from zippendo.models.list_org_brands200_response_data_inner import ListOrgBrands200ResponseDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of ListOrgBrands200ResponseDataInner from a JSON string
list_org_brands200_response_data_inner_instance = ListOrgBrands200ResponseDataInner.from_json(json)
# print the JSON string representation of the object
print(ListOrgBrands200ResponseDataInner.to_json())

# convert the object into a dict
list_org_brands200_response_data_inner_dict = list_org_brands200_response_data_inner_instance.to_dict()
# create an instance of ListOrgBrands200ResponseDataInner from a dict
list_org_brands200_response_data_inner_from_dict = ListOrgBrands200ResponseDataInner.from_dict(list_org_brands200_response_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


