# CreateShipment201ResponseParcelsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | Unique parcel identifier. | [optional] 
**weight** | **float** | Parcel weight in the given weight unit. | 
**weight_unit** | **str** | Unit of measurement for parcel weight. | 
**dimensions** | [**CreateShipment201ResponseParcelsInnerDimensions**](CreateShipment201ResponseParcelsInnerDimensions.md) |  | 
**order_lines** | [**List[CreateShipment201ResponseParcelsInnerOrderLinesInner]**](CreateShipment201ResponseParcelsInnerOrderLinesInner.md) | Order lines contained in this parcel. | 
**tracking_number** | **str** | Carrier tracking number for this parcel. | [optional] 
**tracking_url** | **str** | Public carrier tracking URL for this parcel. | [optional] 
**label_free_code** | **str** | Label-free drop-off code for the parcel. | [optional] 
**qr_code_link** | **str** | DEPRECATED — use &#x60;qrCodeDataUri&#x60; (embeddable data URI) or &#x60;qrCodeUrl&#x60; (hosted link). Catch-all that carries whichever applies, kept populated for backwards compatibility during the migration and until it is disabled. | [optional] 
**qr_code_data_uri** | **str** | Embeddable &#x60;data:&#x60; URI of the QR code image for label-free drop-off — base64 image bytes you can drop straight into an &lt;img&gt;/email. Null when the carrier returns a hosted link instead (see &#x60;qrCodeUrl&#x60;). | [optional] 
**qr_code_url** | **str** | Carrier-hosted URL of the QR code image for label-free drop-off, returned by carriers (e.g. Bring) that link to the image rather than embedding it. Null when the carrier returns embeddable bytes (see &#x60;qrCodeDataUri&#x60;). | [optional] 

## Example

```python
from zippendo.models.create_shipment201_response_parcels_inner import CreateShipment201ResponseParcelsInner

# TODO update the JSON string below
json = "{}"
# create an instance of CreateShipment201ResponseParcelsInner from a JSON string
create_shipment201_response_parcels_inner_instance = CreateShipment201ResponseParcelsInner.from_json(json)
# print the JSON string representation of the object
print(CreateShipment201ResponseParcelsInner.to_json())

# convert the object into a dict
create_shipment201_response_parcels_inner_dict = create_shipment201_response_parcels_inner_instance.to_dict()
# create an instance of CreateShipment201ResponseParcelsInner from a dict
create_shipment201_response_parcels_inner_from_dict = CreateShipment201ResponseParcelsInner.from_dict(create_shipment201_response_parcels_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


