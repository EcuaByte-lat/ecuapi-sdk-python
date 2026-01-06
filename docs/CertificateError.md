# CertificateError


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**error** | [**CertificateErrorError**](CertificateErrorError.md) |  | 

## Example

```python
from ecuapi.models.certificate_error import CertificateError

# TODO update the JSON string below
json = "{}"
# create an instance of CertificateError from a JSON string
certificate_error_instance = CertificateError.from_json(json)
# print the JSON string representation of the object
print(CertificateError.to_json())

# convert the object into a dict
certificate_error_dict = certificate_error_instance.to_dict()
# create an instance of CertificateError from a dict
certificate_error_from_dict = CertificateError.from_dict(certificate_error_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


