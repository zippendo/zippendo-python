# CreateShipment201ResponseDocumentsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | Unique document identifier. | 
**shipment_id** | **str** | Identifier of the shipment this document belongs to. | 
**document_type** | **str** | Type of shipment document. | 
**format** | **str** | File format of the document content. | 
**content** | **str** | Base64-encoded document/label content. | 
**size** | **str** | Physical print size of the document. | [default to 'A4']
**created_at** | **str** | Timestamp when the document was created. | 
**updated_at** | **str** | Timestamp when the document was last updated. | 

## Example

```python
from zippendo.models.create_shipment201_response_documents_inner import CreateShipment201ResponseDocumentsInner

# TODO update the JSON string below
json = "{}"
# create an instance of CreateShipment201ResponseDocumentsInner from a JSON string
create_shipment201_response_documents_inner_instance = CreateShipment201ResponseDocumentsInner.from_json(json)
# print the JSON string representation of the object
print(CreateShipment201ResponseDocumentsInner.to_json())

# convert the object into a dict
create_shipment201_response_documents_inner_dict = create_shipment201_response_documents_inner_instance.to_dict()
# create an instance of CreateShipment201ResponseDocumentsInner from a dict
create_shipment201_response_documents_inner_from_dict = CreateShipment201ResponseDocumentsInner.from_dict(create_shipment201_response_documents_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


