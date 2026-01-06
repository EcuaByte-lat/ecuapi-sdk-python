# CertificateUploadResponseMeta


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**request_id** | **str** |  | 
**timestamp** | **str** |  | 

## Example

```python
from ecuapi.models.certificate_upload_response_meta import CertificateUploadResponseMeta

# TODO update the JSON string below
json = "{}"
# create an instance of CertificateUploadResponseMeta from a JSON string
certificate_upload_response_meta_instance = CertificateUploadResponseMeta.from_json(json)
# print the JSON string representation of the object
print(CertificateUploadResponseMeta.to_json())

# convert the object into a dict
certificate_upload_response_meta_dict = certificate_upload_response_meta_instance.to_dict()
# create an instance of CertificateUploadResponseMeta from a dict
certificate_upload_response_meta_from_dict = CertificateUploadResponseMeta.from_dict(certificate_upload_response_meta_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


