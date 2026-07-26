# CreateShippingRule201Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** | Unique shipping rule identifier | 
**name** | **str** | Shipping rule name | 
**description** | **str** | Optional description | 
**direction** | **str** | Whether this rule is for outbound or inbound (return) shipments | [default to 'outbound']
**carrier_id** | **str** | Carrier ID | 
**product_id** | **str** | Product ID from carrier | 
**services** | **List[str]** | List of selected services | 
**additional_parameters** | [**List[ListShippingRules200ResponseDataInnerAdditionalParametersInner]**](ListShippingRules200ResponseDataInnerAdditionalParametersInner.md) | Carrier-specific extra parameters. DEPRECATED array form &#x60;[{ name, val }]&#x60; where &#x60;name&#x60; is the carrier parameter &#x60;key&#x60; (from the product&#39;s &#x60;additionalParameters[].key&#x60;, e.g. &#x60;returnFunctionality&#x60;) and &#x60;val&#x60; is the stringified value. This will change to a &#x60;{ key: value }&#x60; object in a future version — writes already accept either shape. | 
**address_id** | **str** | Sender address ID | 
**receiving_countries** | **List[str]** | List of supported country codes | 
**email_notification** | **bool** | Send email notification to recipient | [default to False]
**phone_notification** | **bool** | Send SMS notification to recipient | [default to False]
**min_weight** | **float** | Minimum required weight in kg. Orders below this are excluded from the rule. | 
**max_weight** | **float** | Maximum allowed weight in kg. Orders exceeding this are excluded from the rule. | 
**min_order_value** | **float** | Minimum required order value in currency units. Orders below this are excluded from the rule. | 
**max_order_value** | **float** | Maximum allowed order value in currency units. Orders exceeding this are excluded from the rule. | 
**conditions** | [**List[ListShippingRules200ResponseDataInnerConditionsInner]**](ListShippingRules200ResponseDataInnerConditionsInner.md) | Rule conditions (weight/price/quantity) | 
**generate_proforma_invoice** | **bool** | Generate proforma invoice for shipments | [default to False]
**generate_commercial_invoice** | **bool** | Generate commercial invoice for international shipments | [default to False]
**generate_packing_list** | **bool** | Generate packing slip with package and item details | [default to False]
**auto_print_labels** | **bool** | Automatically print labels when shipment is sent | [default to False]
**auto_print_documents** | **bool** | Automatically print documents when shipment is sent | [default to False]
**label_printer_id** | **str** | ID of the label printer | 
**document_printer_id** | **str** | ID of the document printer | 
**return_shipping_rule_id** | **str** | ID of the return shipping rule | 
**auto_create_return_shipment** | **bool** | Automatically create and send a return shipment on dispatch | [default to False]
**org_id** | **str** | Owning organization ID | 
**created_at** | **str** | Creation timestamp (ISO 8601) | 
**updated_at** | **str** | Last update timestamp (ISO 8601) | 

## Example

```python
from zippendo.models.create_shipping_rule201_response import CreateShippingRule201Response

# TODO update the JSON string below
json = "{}"
# create an instance of CreateShippingRule201Response from a JSON string
create_shipping_rule201_response_instance = CreateShippingRule201Response.from_json(json)
# print the JSON string representation of the object
print(CreateShippingRule201Response.to_json())

# convert the object into a dict
create_shipping_rule201_response_dict = create_shipping_rule201_response_instance.to_dict()
# create an instance of CreateShippingRule201Response from a dict
create_shipping_rule201_response_from_dict = CreateShippingRule201Response.from_dict(create_shipping_rule201_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


