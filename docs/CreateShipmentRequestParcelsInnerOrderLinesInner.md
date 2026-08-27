# CreateShipmentRequestParcelsInnerOrderLinesInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | Unique order line identifier. | [optional] 
**sku** | **str** | Stock keeping unit of the product. Optional — not every webshop assigns SKUs. | [optional] 
**quantity** | **int** | Number of units in this order line. | 
**description** | **str** | Human-readable product description. | [optional] 
**unit_price** | **float** | Price per unit in the order line currency. | [optional] 
**currency** | **str** | ISO 4217 currency code. | [optional] 
**vat_percent** | **float** | VAT percentage applied to the unit price. | [optional] 
**location** | **str** | Warehouse picking location. | [optional] 
**country_of_origin** | **str** | ISO 3166-1 alpha-2 country of origin. | [optional] 
**tarrif_number** | **str** | Customs tariff (HS) code. | [optional] 

## Example

```python
from zippendo.models.create_shipment_request_parcels_inner_order_lines_inner import CreateShipmentRequestParcelsInnerOrderLinesInner

# TODO update the JSON string below
json = "{}"
# create an instance of CreateShipmentRequestParcelsInnerOrderLinesInner from a JSON string
create_shipment_request_parcels_inner_order_lines_inner_instance = CreateShipmentRequestParcelsInnerOrderLinesInner.from_json(json)
# print the JSON string representation of the object
print(CreateShipmentRequestParcelsInnerOrderLinesInner.to_json())

# convert the object into a dict
create_shipment_request_parcels_inner_order_lines_inner_dict = create_shipment_request_parcels_inner_order_lines_inner_instance.to_dict()
# create an instance of CreateShipmentRequestParcelsInnerOrderLinesInner from a dict
create_shipment_request_parcels_inner_order_lines_inner_from_dict = CreateShipmentRequestParcelsInnerOrderLinesInner.from_dict(create_shipment_request_parcels_inner_order_lines_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


