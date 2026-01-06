# InvoiceItem


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **str** |  | [optional] 
**description** | **str** |  | 
**quantity** | **float** |  | 
**unit_price** | **int** | Price in cents | 
**discount** | **int** |  | [optional] [default to 0]
**tax_code** | **str** | SRI tax code | 

## Example

```python
from ecuapi.models.invoice_item import InvoiceItem

# TODO update the JSON string below
json = "{}"
# create an instance of InvoiceItem from a JSON string
invoice_item_instance = InvoiceItem.from_json(json)
# print the JSON string representation of the object
print(InvoiceItem.to_json())

# convert the object into a dict
invoice_item_dict = invoice_item_instance.to_dict()
# create an instance of InvoiceItem from a dict
invoice_item_from_dict = InvoiceItem.from_dict(invoice_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


