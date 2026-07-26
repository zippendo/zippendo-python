# SplitShipmentParcelRequestParcelsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | Existing parcel ID to update. Omit to create a new parcel. | [optional] 
**order_lines** | [**List[BatchSplitShipmentRequestShipmentsInnerOrderLinesInner]**](BatchSplitShipmentRequestShipmentsInnerOrderLinesInner.md) | Order lines and quantities to place in this parcel. | 

## Example

```python
from zippendo.models.split_shipment_parcel_request_parcels_inner import SplitShipmentParcelRequestParcelsInner

# TODO update the JSON string below
json = "{}"
# create an instance of SplitShipmentParcelRequestParcelsInner from a JSON string
split_shipment_parcel_request_parcels_inner_instance = SplitShipmentParcelRequestParcelsInner.from_json(json)
# print the JSON string representation of the object
print(SplitShipmentParcelRequestParcelsInner.to_json())

# convert the object into a dict
split_shipment_parcel_request_parcels_inner_dict = split_shipment_parcel_request_parcels_inner_instance.to_dict()
# create an instance of SplitShipmentParcelRequestParcelsInner from a dict
split_shipment_parcel_request_parcels_inner_from_dict = SplitShipmentParcelRequestParcelsInner.from_dict(split_shipment_parcel_request_parcels_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


