# CreateShippingQuoteRequestDestination


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**country** | **str** | ISO 3166-1 alpha-2 country code | 
**postal_code** | **str** | Postal/ZIP code | [optional] 
**province** | **str** | State/province code | [optional] 
**city** | **str** | City name | [optional] 
**address1** | **str** | Street address line 1 | [optional] 
**address2** | **str** | Street address line 2 | [optional] 

## Example

```python
from zippendo.models.create_shipping_quote_request_destination import CreateShippingQuoteRequestDestination

# TODO update the JSON string below
json = "{}"
# create an instance of CreateShippingQuoteRequestDestination from a JSON string
create_shipping_quote_request_destination_instance = CreateShippingQuoteRequestDestination.from_json(json)
# print the JSON string representation of the object
print(CreateShippingQuoteRequestDestination.to_json())

# convert the object into a dict
create_shipping_quote_request_destination_dict = create_shipping_quote_request_destination_instance.to_dict()
# create an instance of CreateShippingQuoteRequestDestination from a dict
create_shipping_quote_request_destination_from_dict = CreateShippingQuoteRequestDestination.from_dict(create_shipping_quote_request_destination_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


