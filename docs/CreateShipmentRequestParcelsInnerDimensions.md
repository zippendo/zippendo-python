# CreateShipmentRequestParcelsInnerDimensions


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**length** | **float** | Parcel length in centimetres. | 
**width** | **float** | Parcel width in centimetres. | 
**height** | **float** | Parcel height in centimetres. | 

## Example

```python
from zippendo.models.create_shipment_request_parcels_inner_dimensions import CreateShipmentRequestParcelsInnerDimensions

# TODO update the JSON string below
json = "{}"
# create an instance of CreateShipmentRequestParcelsInnerDimensions from a JSON string
create_shipment_request_parcels_inner_dimensions_instance = CreateShipmentRequestParcelsInnerDimensions.from_json(json)
# print the JSON string representation of the object
print(CreateShipmentRequestParcelsInnerDimensions.to_json())

# convert the object into a dict
create_shipment_request_parcels_inner_dimensions_dict = create_shipment_request_parcels_inner_dimensions_instance.to_dict()
# create an instance of CreateShipmentRequestParcelsInnerDimensions from a dict
create_shipment_request_parcels_inner_dimensions_from_dict = CreateShipmentRequestParcelsInnerDimensions.from_dict(create_shipment_request_parcels_inner_dimensions_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


