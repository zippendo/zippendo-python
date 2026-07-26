# CreateShippingQuote200ResponseRatesInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**service_name** | **str** | Display name of the shipping option | 
**service_code** | **str** | Unique identifier for this shipping option | 
**total_price** | **str** | Total shipping price in cents as string | 
**currency** | **str** | ISO 4217 currency code | 
**description** | **str** | Optional description | [optional] 
**min_delivery_date** | **str** | Minimum delivery date (ISO 8601) | [optional] 
**max_delivery_date** | **str** | Maximum delivery date (ISO 8601) | [optional] 
**carrier_name** | **str** | Carrier display name | [optional] 
**carrier_slug** | **str** | Carrier slug identifier | [optional] 
**product_id** | **str** | Carrier product ID | [optional] 
**shipping_rule_id** | **str** | Shipping rule ID that generated this rate | 

## Example

```python
from zippendo.models.create_shipping_quote200_response_rates_inner import CreateShippingQuote200ResponseRatesInner

# TODO update the JSON string below
json = "{}"
# create an instance of CreateShippingQuote200ResponseRatesInner from a JSON string
create_shipping_quote200_response_rates_inner_instance = CreateShippingQuote200ResponseRatesInner.from_json(json)
# print the JSON string representation of the object
print(CreateShippingQuote200ResponseRatesInner.to_json())

# convert the object into a dict
create_shipping_quote200_response_rates_inner_dict = create_shipping_quote200_response_rates_inner_instance.to_dict()
# create an instance of CreateShippingQuote200ResponseRatesInner from a dict
create_shipping_quote200_response_rates_inner_from_dict = CreateShippingQuote200ResponseRatesInner.from_dict(create_shipping_quote200_response_rates_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


