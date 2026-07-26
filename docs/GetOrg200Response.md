# GetOrg200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | Unique organization identifier | 
**name** | **str** | Organization name | 
**slug** | **str** | Organization URL slug (unique identifier) | 
**description** | **str** | Organization description | 
**currency** | **str** | Billing currency (ISO 4217 code) | [default to 'DKK']
**vat_number** | **str** | Company VAT/tax ID for invoices | [optional] 
**billing_email** | **str** | Billing email for invoices | [optional] 
**company_name** | **str** | Legal company name | [optional] 
**address_line1** | **str** | Address line 1 | [optional] 
**address_line2** | **str** | Address line 2 | [optional] 
**city** | **str** | City | [optional] 
**postal_code** | **str** | Postal code | [optional] 
**country** | **str** | Country (ISO 3166-1 alpha-2 code) | [optional] 
**customs** | **Dict[str, str]** | Customs identifiers keyed by type | [optional] 
**created_at** | **str** | Creation timestamp (ISO 8601) | 
**updated_at** | **str** | Last update timestamp (ISO 8601) | 
**count** | [**GetOrg200ResponseCount**](GetOrg200ResponseCount.md) |  | 

## Example

```python
from zippendo.models.get_org200_response import GetOrg200Response

# TODO update the JSON string below
json = "{}"
# create an instance of GetOrg200Response from a JSON string
get_org200_response_instance = GetOrg200Response.from_json(json)
# print the JSON string representation of the object
print(GetOrg200Response.to_json())

# convert the object into a dict
get_org200_response_dict = get_org200_response_instance.to_dict()
# create an instance of GetOrg200Response from a dict
get_org200_response_from_dict = GetOrg200Response.from_dict(get_org200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


