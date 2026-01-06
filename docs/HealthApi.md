# ecuapi.HealthApi

All URIs are relative to *https://api.ecuapi.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_api_info**](HealthApi.md#get_api_info) | **GET** /health | Basic health check
[**get_api_info_0**](HealthApi.md#get_api_info_0) | **GET** /v1/health | Basic health check
[**get_detailed_health**](HealthApi.md#get_detailed_health) | **GET** /health/health | Detailed health check
[**get_detailed_health_0**](HealthApi.md#get_detailed_health_0) | **GET** /v1/health/health | Detailed health check


# **get_api_info**
> HealthResponse get_api_info()

Basic health check

### Example


```python
import ecuapi
from ecuapi.models.health_response import HealthResponse
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
    api_instance = ecuapi.HealthApi(api_client)

    try:
        # Basic health check
        api_response = api_instance.get_api_info()
        print("The response of HealthApi->get_api_info:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling HealthApi->get_api_info: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**HealthResponse**](HealthResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | API is healthy |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_api_info_0**
> HealthResponse get_api_info_0()

Basic health check

### Example


```python
import ecuapi
from ecuapi.models.health_response import HealthResponse
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
    api_instance = ecuapi.HealthApi(api_client)

    try:
        # Basic health check
        api_response = api_instance.get_api_info_0()
        print("The response of HealthApi->get_api_info_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling HealthApi->get_api_info_0: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**HealthResponse**](HealthResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | API is healthy |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_detailed_health**
> HealthResponse get_detailed_health()

Detailed health check

Comprehensive health check including database and storage status

### Example


```python
import ecuapi
from ecuapi.models.health_response import HealthResponse
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
    api_instance = ecuapi.HealthApi(api_client)

    try:
        # Detailed health check
        api_response = api_instance.get_detailed_health()
        print("The response of HealthApi->get_detailed_health:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling HealthApi->get_detailed_health: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**HealthResponse**](HealthResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | All systems healthy |  -  |
**503** | One or more systems degraded |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_detailed_health_0**
> HealthResponse get_detailed_health_0()

Detailed health check

Comprehensive health check including database and storage status

### Example


```python
import ecuapi
from ecuapi.models.health_response import HealthResponse
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
    api_instance = ecuapi.HealthApi(api_client)

    try:
        # Detailed health check
        api_response = api_instance.get_detailed_health_0()
        print("The response of HealthApi->get_detailed_health_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling HealthApi->get_detailed_health_0: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**HealthResponse**](HealthResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | All systems healthy |  -  |
**503** | One or more systems degraded |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

