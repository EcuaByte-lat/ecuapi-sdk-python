# ecuapi.InvoicesApi

All URIs are relative to *https://api.ecuapi.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**authorize_invoice**](InvoicesApi.md#authorize_invoice) | **POST** /v1/invoices/{id}/authorize | Authorize invoice
[**create_invoice**](InvoicesApi.md#create_invoice) | **POST** /v1/invoices | Create invoice
[**get_invoice**](InvoicesApi.md#get_invoice) | **GET** /v1/invoices/{id} | Get invoice by ID
[**get_invoice_pdf**](InvoicesApi.md#get_invoice_pdf) | **GET** /v1/invoices/{id}/pdf | Download RIDE PDF
[**get_invoice_xml**](InvoicesApi.md#get_invoice_xml) | **GET** /v1/invoices/{id}/xml | Download signed XML
[**list_invoices**](InvoicesApi.md#list_invoices) | **GET** /v1/invoices | List invoices
[**send_invoice**](InvoicesApi.md#send_invoice) | **POST** /v1/invoices/{id}/send | Send invoice to SRI
[**void_invoice**](InvoicesApi.md#void_invoice) | **DELETE** /v1/invoices/{id} | Void invoice


# **authorize_invoice**
> AuthorizeInvoiceResponse authorize_invoice(id)

Authorize invoice

Check authorization status with SRI after sending

### Example


```python
import ecuapi
from ecuapi.models.authorize_invoice_response import AuthorizeInvoiceResponse
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
    api_instance = ecuapi.InvoicesApi(api_client)
    id = 'inv_abc123' # str | 

    try:
        # Authorize invoice
        api_response = api_instance.authorize_invoice(id)
        print("The response of InvoicesApi->authorize_invoice:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InvoicesApi->authorize_invoice: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

### Return type

[**AuthorizeInvoiceResponse**](AuthorizeInvoiceResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Authorization result |  -  |
**400** | Invoice has no access key |  -  |
**404** | Invoice not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_invoice**
> CreateInvoiceResponse create_invoice(create_invoice_request=create_invoice_request)

Create invoice

Create a new invoice in draft status

### Example


```python
import ecuapi
from ecuapi.models.create_invoice_request import CreateInvoiceRequest
from ecuapi.models.create_invoice_response import CreateInvoiceResponse
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
    api_instance = ecuapi.InvoicesApi(api_client)
    create_invoice_request = ecuapi.CreateInvoiceRequest() # CreateInvoiceRequest |  (optional)

    try:
        # Create invoice
        api_response = api_instance.create_invoice(create_invoice_request=create_invoice_request)
        print("The response of InvoicesApi->create_invoice:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InvoicesApi->create_invoice: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **create_invoice_request** | [**CreateInvoiceRequest**](CreateInvoiceRequest.md)|  | [optional] 

### Return type

[**CreateInvoiceResponse**](CreateInvoiceResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Invoice created successfully |  -  |
**400** | Invalid request |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_invoice**
> InvoiceDetailResponse get_invoice(id)

Get invoice by ID

Retrieve a single invoice with all its items

### Example


```python
import ecuapi
from ecuapi.models.invoice_detail_response import InvoiceDetailResponse
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
    api_instance = ecuapi.InvoicesApi(api_client)
    id = 'inv_abc123' # str | 

    try:
        # Get invoice by ID
        api_response = api_instance.get_invoice(id)
        print("The response of InvoicesApi->get_invoice:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InvoicesApi->get_invoice: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

### Return type

[**InvoiceDetailResponse**](InvoiceDetailResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Invoice details |  -  |
**404** | Invoice not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_invoice_pdf**
> object get_invoice_pdf(id)

Download RIDE PDF

Generate and download the RIDE PDF for an invoice

### Example


```python
import ecuapi
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
    api_instance = ecuapi.InvoicesApi(api_client)
    id = 'inv_abc123' # str | 

    try:
        # Download RIDE PDF
        api_response = api_instance.get_invoice_pdf(id)
        print("The response of InvoicesApi->get_invoice_pdf:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InvoicesApi->get_invoice_pdf: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

### Return type

**object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/pdf, application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | PDF file |  -  |
**404** | Invoice not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_invoice_xml**
> object get_invoice_xml(id)

Download signed XML

Download the signed XML document for an invoice

### Example


```python
import ecuapi
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
    api_instance = ecuapi.InvoicesApi(api_client)
    id = 'inv_abc123' # str | 

    try:
        # Download signed XML
        api_response = api_instance.get_invoice_xml(id)
        print("The response of InvoicesApi->get_invoice_xml:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InvoicesApi->get_invoice_xml: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

### Return type

**object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/xml, application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | XML file |  -  |
**404** | Invoice or XML not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_invoices**
> InvoiceListResponse list_invoices(status=status, page=page, limit=limit)

List invoices

Retrieve a paginated list of invoices for the organization

### Example


```python
import ecuapi
from ecuapi.models.invoice_list_response import InvoiceListResponse
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
    api_instance = ecuapi.InvoicesApi(api_client)
    status = 'authorized' # str |  (optional)
    page = 1 # int |  (optional) (default to 1)
    limit = 20 # int |  (optional) (default to 20)

    try:
        # List invoices
        api_response = api_instance.list_invoices(status=status, page=page, limit=limit)
        print("The response of InvoicesApi->list_invoices:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InvoicesApi->list_invoices: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **status** | **str**|  | [optional] 
 **page** | **int**|  | [optional] [default to 1]
 **limit** | **int**|  | [optional] [default to 20]

### Return type

[**InvoiceListResponse**](InvoiceListResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | List of invoices |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **send_invoice**
> SendInvoiceResponse send_invoice(id)

Send invoice to SRI

Sign and send the invoice to SRI for processing

### Example


```python
import ecuapi
from ecuapi.models.send_invoice_response import SendInvoiceResponse
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
    api_instance = ecuapi.InvoicesApi(api_client)
    id = 'inv_abc123' # str | 

    try:
        # Send invoice to SRI
        api_response = api_instance.send_invoice(id)
        print("The response of InvoicesApi->send_invoice:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InvoicesApi->send_invoice: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

### Return type

[**SendInvoiceResponse**](SendInvoiceResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Invoice sent successfully |  -  |
**400** | Invalid invoice status or missing certificate |  -  |
**404** | Invoice not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **void_invoice**
> void_invoice(id)

Void invoice

Void/cancel an invoice (not yet implemented)

### Example


```python
import ecuapi
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
    api_instance = ecuapi.InvoicesApi(api_client)
    id = 'inv_abc123' # str | 

    try:
        # Void invoice
        api_instance.void_invoice(id)
    except Exception as e:
        print("Exception when calling InvoicesApi->void_invoice: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**501** | Not implemented |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

