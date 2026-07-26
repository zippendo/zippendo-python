# CreateShipment201ResponseTracking


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**url** | **str** | Public carrier tracking URL. | [optional] 
**number** | **str** | Carrier tracking number. | [optional] 
**label_free_code** | **str** | Label-free drop-off code. | [optional] 
**qr_code_link** | **str** | DEPRECATED — use &#x60;qrCodeDataUri&#x60; (embeddable data URI) or &#x60;qrCodeUrl&#x60; (hosted link). Catch-all that carries whichever applies, kept populated for backwards compatibility during the migration and until it is disabled. | [optional] 
**qr_code_data_uri** | **str** | Embeddable &#x60;data:&#x60; URI of the QR code image for label-free drop-off — base64 image bytes you can drop straight into an &lt;img&gt;/email. Null when the carrier returns a hosted link instead (see &#x60;qrCodeUrl&#x60;). | [optional] 
**qr_code_url** | **str** | Carrier-hosted URL of the QR code image for label-free drop-off, returned by carriers (e.g. Bring) that link to the image rather than embedding it. Null when the carrier returns embeddable bytes (see &#x60;qrCodeDataUri&#x60;). | [optional] 

## Example

```python
from zippendo.models.create_shipment201_response_tracking import CreateShipment201ResponseTracking

# TODO update the JSON string below
json = "{}"
# create an instance of CreateShipment201ResponseTracking from a JSON string
create_shipment201_response_tracking_instance = CreateShipment201ResponseTracking.from_json(json)
# print the JSON string representation of the object
print(CreateShipment201ResponseTracking.to_json())

# convert the object into a dict
create_shipment201_response_tracking_dict = create_shipment201_response_tracking_instance.to_dict()
# create an instance of CreateShipment201ResponseTracking from a dict
create_shipment201_response_tracking_from_dict = CreateShipment201ResponseTracking.from_dict(create_shipment201_response_tracking_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


