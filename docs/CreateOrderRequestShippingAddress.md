# CreateOrderRequestShippingAddress

Destination shipping address.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** | Recipient full name. | 
**attention** | **str** | Attention / care-of line. | [optional] 
**company** | **str** | Company name. | [optional] 
**address1** | **str** | Street address line 1. | 
**address2** | **str** | Street address line 2. | [optional] 
**city** | **str** | City name. | 
**province** | **str** | Province or region name. | [optional] 
**province_code** | **str** | Province or region code. | [optional] 
**postal_code** | **str** | Postal code. | 
**country** | **str** | Country name. | [optional] 
**country_code** | **str** | ISO 3166-1 alpha-2 country code. | 
**phone** | **str** | Recipient phone number. | [optional] 
**email** | **str** | Recipient email address. | [optional] 

## Example

```python
from zippendo.models.create_order_request_shipping_address import CreateOrderRequestShippingAddress

# TODO update the JSON string below
json = "{}"
# create an instance of CreateOrderRequestShippingAddress from a JSON string
create_order_request_shipping_address_instance = CreateOrderRequestShippingAddress.from_json(json)
# print the JSON string representation of the object
print(CreateOrderRequestShippingAddress.to_json())

# convert the object into a dict
create_order_request_shipping_address_dict = create_order_request_shipping_address_instance.to_dict()
# create an instance of CreateOrderRequestShippingAddress from a dict
create_order_request_shipping_address_from_dict = CreateOrderRequestShippingAddress.from_dict(create_order_request_shipping_address_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


