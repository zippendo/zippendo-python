# UpdateOrgBrandRequest


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
**name** | **str** | Brand display name | [optional] 
**slug** | **str** | URL-safe identifier, unique within the org | [optional] 
**use_org_customs** | **bool** | Whether this brand ships under the organization&#39;s fiscal identity. True (the default) declares the organization&#39;s VAT number and customs identifiers and ignores the brand&#39;s own. False makes the brand&#39;s own values the sole source — nothing falls back to the organization, so an identifier the brand has not set is not declared at all. | [optional] 

## Example

```python
from zippendo.models.update_org_brand_request import UpdateOrgBrandRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateOrgBrandRequest from a JSON string
update_org_brand_request_instance = UpdateOrgBrandRequest.from_json(json)
# print the JSON string representation of the object
print(UpdateOrgBrandRequest.to_json())

# convert the object into a dict
update_org_brand_request_dict = update_org_brand_request_instance.to_dict()
# create an instance of UpdateOrgBrandRequest from a dict
update_org_brand_request_from_dict = UpdateOrgBrandRequest.from_dict(update_org_brand_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


