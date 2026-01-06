# CertificateErrorError


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **str** |  | 
**message** | **str** |  | 

## Example

```python
from ecuapi.models.certificate_error_error import CertificateErrorError

# TODO update the JSON string below
json = "{}"
# create an instance of CertificateErrorError from a JSON string
certificate_error_error_instance = CertificateErrorError.from_json(json)
# print the JSON string representation of the object
print(CertificateErrorError.to_json())

# convert the object into a dict
certificate_error_error_dict = certificate_error_error_instance.to_dict()
# create an instance of CertificateErrorError from a dict
certificate_error_error_from_dict = CertificateErrorError.from_dict(certificate_error_error_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


