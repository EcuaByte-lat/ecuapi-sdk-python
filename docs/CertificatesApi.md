# ecuapi.CertificatesApi

All URIs are relative to *https://api.ecuapi.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**list_certificates**](CertificatesApi.md#list_certificates) | **GET** /v1/certificates | List certificates
[**upload_certificate**](CertificatesApi.md#upload_certificate) | **POST** /v1/certificates/upload | Upload P12 certificate


# **list_certificates**
> CertificateListResponse list_certificates()

List certificates

List all certificates for the organization

### Example


```python
import ecuapi
from ecuapi.models.certificate_list_response import CertificateListResponse
from ecuapi.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.ecuapi.com
# See configuration.py for a list of all supported configuration parameters.
configuration = ecuapi.Configuration(
    host = "https://api.ecuapi.com"
)


# Enter a context with an instance of the API client
with ecuapi.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = ecuapi.CertificatesApi(api_client)

    try:
        # List certificates
        api_response = api_instance.list_certificates()
        print("The response of CertificatesApi->list_certificates:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CertificatesApi->list_certificates: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**CertificateListResponse**](CertificateListResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | List of certificates |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **upload_certificate**
> CertificateUploadResponse upload_certificate(password, file=file, alias=alias)

Upload P12 certificate

Upload a P12 electronic signature certificate for signing invoices

### Example


```python
import ecuapi
from ecuapi.models.certificate_upload_response import CertificateUploadResponse
from ecuapi.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.ecuapi.com
# See configuration.py for a list of all supported configuration parameters.
configuration = ecuapi.Configuration(
    host = "https://api.ecuapi.com"
)


# Enter a context with an instance of the API client
with ecuapi.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = ecuapi.CertificatesApi(api_client)
    password = 'password_example' # str | 
    file = None # bytearray | P12 certificate file (optional)
    alias = 'alias_example' # str |  (optional)

    try:
        # Upload P12 certificate
        api_response = api_instance.upload_certificate(password, file=file, alias=alias)
        print("The response of CertificatesApi->upload_certificate:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CertificatesApi->upload_certificate: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **password** | **str**|  | 
 **file** | **bytearray**| P12 certificate file | [optional] 
 **alias** | **str**|  | [optional] 

### Return type

[**CertificateUploadResponse**](CertificateUploadResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Certificate uploaded successfully |  -  |
**400** | Invalid file or certificate |  -  |
**401** | Invalid password |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

