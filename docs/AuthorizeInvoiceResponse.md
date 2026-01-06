# AuthorizeInvoiceResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**AuthorizeInvoiceResponseData**](AuthorizeInvoiceResponseData.md) |  | 
**meta** | [**Meta**](Meta.md) |  | 

## Example

```python
from ecuapi.models.authorize_invoice_response import AuthorizeInvoiceResponse

# TODO update the JSON string below
json = "{}"
# create an instance of AuthorizeInvoiceResponse from a JSON string
authorize_invoice_response_instance = AuthorizeInvoiceResponse.from_json(json)
# print the JSON string representation of the object
print(AuthorizeInvoiceResponse.to_json())

# convert the object into a dict
authorize_invoice_response_dict = authorize_invoice_response_instance.to_dict()
# create an instance of AuthorizeInvoiceResponse from a dict
authorize_invoice_response_from_dict = AuthorizeInvoiceResponse.from_dict(authorize_invoice_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


