# ListCarrierProductServicePoints200ResponseInnerAddress

Postal address of the service point

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**address1** | **str** | Street address line 1 | 
**address2** | **str** | Street address line 2 | [optional] 
**postal_code** | **str** | Postal code | 
**state** | **str** | State or region | [optional] 
**city** | **str** | City name | 
**country_code** | **str** | ISO 3166-1 alpha-2 country code | 

## Example

```python
from zippendo.models.list_carrier_product_service_points200_response_inner_address import ListCarrierProductServicePoints200ResponseInnerAddress

# TODO update the JSON string below
json = "{}"
# create an instance of ListCarrierProductServicePoints200ResponseInnerAddress from a JSON string
list_carrier_product_service_points200_response_inner_address_instance = ListCarrierProductServicePoints200ResponseInnerAddress.from_json(json)
# print the JSON string representation of the object
print(ListCarrierProductServicePoints200ResponseInnerAddress.to_json())

# convert the object into a dict
list_carrier_product_service_points200_response_inner_address_dict = list_carrier_product_service_points200_response_inner_address_instance.to_dict()
# create an instance of ListCarrierProductServicePoints200ResponseInnerAddress from a dict
list_carrier_product_service_points200_response_inner_address_from_dict = ListCarrierProductServicePoints200ResponseInnerAddress.from_dict(list_carrier_product_service_points200_response_inner_address_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


