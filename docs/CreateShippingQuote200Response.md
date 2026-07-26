# CreateShippingQuote200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**rates** | [**List[CreateShippingQuote200ResponseRatesInner]**](CreateShippingQuote200ResponseRatesInner.md) | Available shipping rates | 

## Example

```python
from zippendo.models.create_shipping_quote200_response import CreateShippingQuote200Response

# TODO update the JSON string below
json = "{}"
# create an instance of CreateShippingQuote200Response from a JSON string
create_shipping_quote200_response_instance = CreateShippingQuote200Response.from_json(json)
# print the JSON string representation of the object
print(CreateShippingQuote200Response.to_json())

# convert the object into a dict
create_shipping_quote200_response_dict = create_shipping_quote200_response_instance.to_dict()
# create an instance of CreateShippingQuote200Response from a dict
create_shipping_quote200_response_from_dict = CreateShippingQuote200Response.from_dict(create_shipping_quote200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


