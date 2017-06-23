# swagger_client.DefaultApi

All URIs are relative to *https://virtserver.swaggerhub.com/vinayski/Regression/1.0.0*

Method | HTTP request | Description
------------- | ------------- | -------------
[**predict_post**](DefaultApi.md#predict_post) | **POST** /predict | Predicts from test data
[**train_post**](DefaultApi.md#train_post) | **POST** /train | trains the model


# **predict_post**
> predict_post(test=test)

Predicts from test data

### Example 
```python
from __future__ import print_statement
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = swagger_client.DefaultApi()
test = '/path/to/file.txt' # file | Test file for predictions (optional)

try: 
    # Predicts from test data
    api_instance.predict_post(test=test)
except ApiException as e:
    print("Exception when calling DefaultApi->predict_post: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **test** | **file**| Test file for predictions | [optional] 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **train_post**
> train_post(train=train)

trains the model

### Example 
```python
from __future__ import print_statement
import time
import swagger_client
from swagger_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = swagger_client.DefaultApi()
train = '/path/to/file.txt' # file | Training file (optional)

try: 
    # trains the model
    api_instance.train_post(train=train)
except ApiException as e:
    print("Exception when calling DefaultApi->train_post: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **train** | **file**| Training file | [optional] 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

