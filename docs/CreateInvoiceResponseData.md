# CreateInvoiceResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**subtotal** | **float** |  | 
**tax_amount** | **float** |  | 
**total** | **float** |  | 
**status** | **str** |  | 

## Example

```python
from ecuapi.models.create_invoice_response_data import CreateInvoiceResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of CreateInvoiceResponseData from a JSON string
create_invoice_response_data_instance = CreateInvoiceResponseData.from_json(json)
# print the JSON string representation of the object
print(CreateInvoiceResponseData.to_json())

# convert the object into a dict
create_invoice_response_data_dict = create_invoice_response_data_instance.to_dict()
# create an instance of CreateInvoiceResponseData from a dict
create_invoice_response_data_from_dict = CreateInvoiceResponseData.from_dict(create_invoice_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


