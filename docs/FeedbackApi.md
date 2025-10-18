# blackman_client.FeedbackApi

All URIs are relative to *https://app.useblackman.ai/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**submit_feedback**](FeedbackApi.md#submit_feedback) | **POST** /v1/feedback | Submit feedback for a completion response


# **submit_feedback**
> SubmitFeedbackResponse submit_feedback(submit_feedback_request)

Submit feedback for a completion response

### Example

* Bearer Authentication (BearerAuth):

```python
import blackman_client
from blackman_client.models.submit_feedback_request import SubmitFeedbackRequest
from blackman_client.models.submit_feedback_response import SubmitFeedbackResponse
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
    api_instance = blackman_client.FeedbackApi(api_client)
    submit_feedback_request = blackman_client.SubmitFeedbackRequest() # SubmitFeedbackRequest | 

    try:
        # Submit feedback for a completion response
        api_response = api_instance.submit_feedback(submit_feedback_request)
        print("The response of FeedbackApi->submit_feedback:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FeedbackApi->submit_feedback: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **submit_feedback_request** | [**SubmitFeedbackRequest**](SubmitFeedbackRequest.md)|  | 

### Return type

[**SubmitFeedbackResponse**](SubmitFeedbackResponse.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Feedback submitted successfully |  -  |
**401** | Unauthorized |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

