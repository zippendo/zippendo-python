# CreateShipmentRequestPartiesInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** | Role of the party in the shipment. | 
**name** | **str** | Full name or company name of the party. | 
**attention** | **str** | Attention contact at the party. | [optional] 
**address1** | **str** | Primary street address line. | 
**address2** | **str** | Secondary address line. | [optional] 
**postal_code** | **str** | Postal code of the party address. | 
**city** | **str** | City of the party address. | 
**country_code** | **str** | ISO 3166-1 alpha-2 country code. | 
**email** | **str** | Email address of the party. | [optional] 
**phone** | **str** | Phone number of the party in E.164 format. | [optional] 
**attributes** | [**List[CreateShipmentRequestPartiesInnerAttributesInner]**](CreateShipmentRequestPartiesInnerAttributesInner.md) | Additional carrier-specific attributes for the party. | [optional] [default to []]

## Example

```python
from zippendo.models.create_shipment_request_parties_inner import CreateShipmentRequestPartiesInner

# TODO update the JSON string below
json = "{}"
# create an instance of CreateShipmentRequestPartiesInner from a JSON string
create_shipment_request_parties_inner_instance = CreateShipmentRequestPartiesInner.from_json(json)
# print the JSON string representation of the object
print(CreateShipmentRequestPartiesInner.to_json())

# convert the object into a dict
create_shipment_request_parties_inner_dict = create_shipment_request_parties_inner_instance.to_dict()
# create an instance of CreateShipmentRequestPartiesInner from a dict
create_shipment_request_parties_inner_from_dict = CreateShipmentRequestPartiesInner.from_dict(create_shipment_request_parties_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


