# CreateOrgBrandRequest


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
**name** | **str** | Brand display name | 
**slug** | **str** | URL-safe identifier, unique within the org. Derived from the name when omitted. | [optional] 
**use_org_customs** | **bool** | Whether this brand ships under the organization&#39;s fiscal identity. True (the default) declares the organization&#39;s VAT number and customs identifiers and ignores the brand&#39;s own. False makes the brand&#39;s own values the sole source — nothing falls back to the organization, so an identifier the brand has not set is not declared at all. | [optional] 

## Example

```python
from zippendo.models.create_org_brand_request import CreateOrgBrandRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateOrgBrandRequest from a JSON string
create_org_brand_request_instance = CreateOrgBrandRequest.from_json(json)
# print the JSON string representation of the object
print(CreateOrgBrandRequest.to_json())

# convert the object into a dict
create_org_brand_request_dict = create_org_brand_request_instance.to_dict()
# create an instance of CreateOrgBrandRequest from a dict
create_org_brand_request_from_dict = CreateOrgBrandRequest.from_dict(create_org_brand_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


