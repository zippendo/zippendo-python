# CreateShippingRuleRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** | Shipping rule name | 
**description** | **str** | Optional description | [optional] 
**direction** | **str** | Whether this rule is for outbound or inbound (return) shipments | [optional] [default to 'outbound']
**carrier_id** | **str** | Carrier ID | 
**product_id** | **str** | Product ID from carrier | 
**services** | **List[str]** | List of selected services | 
**additional_parameters** | [**CreateShippingRuleRequestAdditionalParameters**](CreateShippingRuleRequestAdditionalParameters.md) |  | [optional] 
**address_id** | **str** | Sender address ID | 
**receiving_countries** | **List[str]** | List of supported country codes | 
**email_notification** | **bool** | Send email notification to recipient | [optional] [default to False]
**phone_notification** | **bool** | Send SMS notification to recipient | [optional] [default to False]
**min_weight** | **float** | Minimum required weight in kg | [optional] 
**max_weight** | **float** | Maximum allowed weight in kg | [optional] 
**min_order_value** | **float** | Minimum required order value in currency units | [optional] 
**max_order_value** | **float** | Maximum allowed order value in currency units | [optional] 
**conditions** | [**List[CreateShippingRuleRequestConditionsInner]**](CreateShippingRuleRequestConditionsInner.md) | Rule conditions (weight/price/quantity) | 
**generate_proforma_invoice** | **bool** | Generate proforma invoice for shipments | [optional] [default to False]
**generate_commercial_invoice** | **bool** | Generate commercial invoice for international shipments | [optional] [default to False]
**generate_packing_list** | **bool** | Generate packing slip with package and item details | [optional] [default to False]
**auto_print_labels** | **bool** | Automatically print labels when shipment is sent | [optional] [default to False]
**auto_print_documents** | **bool** | Automatically print documents when shipment is sent | [optional] [default to False]
**label_printer_id** | **str** | ID of the label printer | [optional] 
**document_printer_id** | **str** | ID of the document printer | [optional] 
**return_shipping_rule_id** | **str** | ID of the return shipping rule | [optional] 
**auto_create_return_shipment** | **bool** | Automatically create and send a return shipment on dispatch | [optional] [default to False]

## Example

```python
from zippendo.models.create_shipping_rule_request import CreateShippingRuleRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateShippingRuleRequest from a JSON string
create_shipping_rule_request_instance = CreateShippingRuleRequest.from_json(json)
# print the JSON string representation of the object
print(CreateShippingRuleRequest.to_json())

# convert the object into a dict
create_shipping_rule_request_dict = create_shipping_rule_request_instance.to_dict()
# create an instance of CreateShippingRuleRequest from a dict
create_shipping_rule_request_from_dict = CreateShippingRuleRequest.from_dict(create_shipping_rule_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


