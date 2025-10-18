# blackman_client.SemanticCacheApi

All URIs are relative to *https://app.useblackman.ai/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_config**](SemanticCacheApi.md#get_config) | **GET** /v1/semantic-cache/config | Get semantic cache configuration for the current account
[**get_stats**](SemanticCacheApi.md#get_stats) | **GET** /v1/semantic-cache/stats | Get semantic cache statistics including hit rate and savings
[**invalidate_all**](SemanticCacheApi.md#invalidate_all) | **DELETE** /v1/semantic-cache/invalidate | Invalidate all cache entries for the current account
[**update_config**](SemanticCacheApi.md#update_config) | **PUT** /v1/semantic-cache/config | Update semantic cache configuration for the current account


# **get_config**
> SemanticCacheConfig get_config()

Get semantic cache configuration for the current account

### Example

* Bearer Authentication (BearerAuth):

```python
import blackman_client
from blackman_client.models.semantic_cache_config import SemanticCacheConfig
from blackman_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://app.useblackman.ai/v1
# See configuration.py for a list of all supported configuration parameters.
configuration = blackman_client.Configuration(
    host = "https://app.useblackman.ai/v1"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization: BearerAuth
configuration = blackman_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with blackman_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = blackman_client.SemanticCacheApi(api_client)

    try:
        # Get semantic cache configuration for the current account
        api_response = api_instance.get_config()
        print("The response of SemanticCacheApi->get_config:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SemanticCacheApi->get_config: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**SemanticCacheConfig**](SemanticCacheConfig.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Cache configuration retrieved successfully |  -  |
**401** | Unauthorized |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_stats**
> SemanticCacheStats get_stats()

Get semantic cache statistics including hit rate and savings

### Example

* Bearer Authentication (BearerAuth):

```python
import blackman_client
from blackman_client.models.semantic_cache_stats import SemanticCacheStats
from blackman_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://app.useblackman.ai/v1
# See configuration.py for a list of all supported configuration parameters.
configuration = blackman_client.Configuration(
    host = "https://app.useblackman.ai/v1"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization: BearerAuth
configuration = blackman_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with blackman_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = blackman_client.SemanticCacheApi(api_client)

    try:
        # Get semantic cache statistics including hit rate and savings
        api_response = api_instance.get_stats()
        print("The response of SemanticCacheApi->get_stats:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SemanticCacheApi->get_stats: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**SemanticCacheStats**](SemanticCacheStats.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Cache statistics retrieved successfully |  -  |
**401** | Unauthorized |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **invalidate_all**
> InvalidateResponse invalidate_all()

Invalidate all cache entries for the current account

### Example

* Bearer Authentication (BearerAuth):

```python
import blackman_client
from blackman_client.models.invalidate_response import InvalidateResponse
from blackman_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://app.useblackman.ai/v1
# See configuration.py for a list of all supported configuration parameters.
configuration = blackman_client.Configuration(
    host = "https://app.useblackman.ai/v1"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization: BearerAuth
configuration = blackman_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with blackman_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = blackman_client.SemanticCacheApi(api_client)

    try:
        # Invalidate all cache entries for the current account
        api_response = api_instance.invalidate_all()
        print("The response of SemanticCacheApi->invalidate_all:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SemanticCacheApi->invalidate_all: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**InvalidateResponse**](InvalidateResponse.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | All cache entries invalidated successfully |  -  |
**401** | Unauthorized |  -  |
**500** | Internal server error |  -  |
**503** | Semantic cache not configured |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_config**
> update_config(semantic_cache_config)

Update semantic cache configuration for the current account

### Example

* Bearer Authentication (BearerAuth):

```python
import blackman_client
from blackman_client.models.semantic_cache_config import SemanticCacheConfig
from blackman_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://app.useblackman.ai/v1
# See configuration.py for a list of all supported configuration parameters.
configuration = blackman_client.Configuration(
    host = "https://app.useblackman.ai/v1"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization: BearerAuth
configuration = blackman_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with blackman_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = blackman_client.SemanticCacheApi(api_client)
    semantic_cache_config = blackman_client.SemanticCacheConfig() # SemanticCacheConfig | 

    try:
        # Update semantic cache configuration for the current account
        api_instance.update_config(semantic_cache_config)
    except Exception as e:
        print("Exception when calling SemanticCacheApi->update_config: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **semantic_cache_config** | [**SemanticCacheConfig**](SemanticCacheConfig.md)|  | 

### Return type

void (empty response body)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**204** | Cache configuration updated successfully |  -  |
**400** | Invalid configuration values |  -  |
**401** | Unauthorized |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

