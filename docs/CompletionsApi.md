# blackman_client.CompletionsApi

All URIs are relative to *https://app.useblackman.ai/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**completions**](CompletionsApi.md#completions) | **POST** /v1/completions | 


# **completions**
> CompletionResponse completions(completion_request, x_provider_api_key=x_provider_api_key)

### Example

* Bearer Authentication (BearerAuth):

```python
import blackman_client
from blackman_client.models.completion_request import CompletionRequest
from blackman_client.models.completion_response import CompletionResponse
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
    api_instance = blackman_client.CompletionsApi(api_client)
    completion_request = blackman_client.CompletionRequest() # CompletionRequest | 
    x_provider_api_key = 'x_provider_api_key_example' # str | Optional provider API key to override stored or system keys (optional)

    try:
        api_response = api_instance.completions(completion_request, x_provider_api_key=x_provider_api_key)
        print("The response of CompletionsApi->completions:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CompletionsApi->completions: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **completion_request** | [**CompletionRequest**](CompletionRequest.md)|  | 
 **x_provider_api_key** | **str**| Optional provider API key to override stored or system keys | [optional] 

### Return type

[**CompletionResponse**](CompletionResponse.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | AI completion response |  -  |
**401** | Unauthorized - missing or invalid authentication token |  -  |
**402** | Payment required - no active subscription |  -  |
**500** | Provider error |  -  |
**503** | Service unavailable - provider API key not configured |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

