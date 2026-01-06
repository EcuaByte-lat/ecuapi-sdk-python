# CreateInvoiceResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**CreateInvoiceResponseData**](CreateInvoiceResponseData.md) |  | 
**meta** | [**Meta**](Meta.md) |  | 

## Example

```python
from ecuapi.models.create_invoice_response import CreateInvoiceResponse

# TODO update the JSON string below
json = "{}"
# create an instance of CreateInvoiceResponse from a JSON string
create_invoice_response_instance = CreateInvoiceResponse.from_json(json)
# print the JSON string representation of the object
print(CreateInvoiceResponse.to_json())

# convert the object into a dict
create_invoice_response_dict = create_invoice_response_instance.to_dict()
# create an instance of CreateInvoiceResponse from a dict
create_invoice_response_from_dict = CreateInvoiceResponse.from_dict(create_invoice_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


