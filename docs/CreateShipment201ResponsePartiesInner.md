# CreateShipment201ResponsePartiesInner


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
**attributes** | [**List[CreateShipment201ResponsePartiesInnerAttributesInner]**](CreateShipment201ResponsePartiesInnerAttributesInner.md) | Additional carrier-specific attributes for the party. | [default to []]

## Example

```python
from zippendo.models.create_shipment201_response_parties_inner import CreateShipment201ResponsePartiesInner

# TODO update the JSON string below
json = "{}"
# create an instance of CreateShipment201ResponsePartiesInner from a JSON string
create_shipment201_response_parties_inner_instance = CreateShipment201ResponsePartiesInner.from_json(json)
# print the JSON string representation of the object
print(CreateShipment201ResponsePartiesInner.to_json())

# convert the object into a dict
create_shipment201_response_parties_inner_dict = create_shipment201_response_parties_inner_instance.to_dict()
# create an instance of CreateShipment201ResponsePartiesInner from a dict
create_shipment201_response_parties_inner_from_dict = CreateShipment201ResponsePartiesInner.from_dict(create_shipment201_response_parties_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


