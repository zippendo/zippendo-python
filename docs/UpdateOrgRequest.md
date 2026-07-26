# UpdateOrgRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** | Organization name | [optional] 
**slug** | **str** | Organization slug | [optional] 
**description** | **str** | Organization description | [optional] 
**currency** | **str** | Billing currency (ISO 4217 code) | [optional] 
**vat_number** | **str** | Company VAT/tax ID for invoices | [optional] 
**overage_enabled** | **bool** | Allow shipments beyond plan limit (overage charges apply) | [optional] 
**billing_email** | **str** | Billing email for invoices | [optional] 
**company_name** | **str** | Legal company name | [optional] 
**address_line1** | **str** | Address line 1 | [optional] 
**address_line2** | **str** | Address line 2 | [optional] 
**city** | **str** | City | [optional] 
**postal_code** | **str** | Postal code | [optional] 
**country** | **str** | Country (ISO 3166-1 alpha-2 code) | [optional] 
**customs** | **Dict[str, str]** | Organization-wide customs identifiers (EORI, IOSS, VOEC, etc.); null clears all | [optional] 

## Example

```python
from zippendo.models.update_org_request import UpdateOrgRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateOrgRequest from a JSON string
update_org_request_instance = UpdateOrgRequest.from_json(json)
# print the JSON string representation of the object
print(UpdateOrgRequest.to_json())

# convert the object into a dict
update_org_request_dict = update_org_request_instance.to_dict()
# create an instance of UpdateOrgRequest from a dict
update_org_request_from_dict = UpdateOrgRequest.from_dict(update_org_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


