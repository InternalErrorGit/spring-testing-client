# PingControllerApi

All URIs are relative to *http://localhost:8080*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**ping**](PingControllerApi.md#ping) | **GET** /api/ping |  |
| [**pong**](PingControllerApi.md#pong) | **GET** /api/pong |  |


<a id="ping"></a>
# **ping**
> String ping()



### Example
```java
// Import classes:
import net.internalerror.invoker.ApiClient;
import net.internalerror.invoker.ApiException;
import net.internalerror.invoker.Configuration;
import net.internalerror.invoker.models.*;
import net.internalerror.api.PingControllerApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://localhost:8080");

    PingControllerApi apiInstance = new PingControllerApi(defaultClient);
    try {
      String result = apiInstance.ping();
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling PingControllerApi#ping");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

**String**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |

<a id="pong"></a>
# **pong**
> String pong()



### Example
```java
// Import classes:
import net.internalerror.invoker.ApiClient;
import net.internalerror.invoker.ApiException;
import net.internalerror.invoker.Configuration;
import net.internalerror.invoker.models.*;
import net.internalerror.api.PingControllerApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://localhost:8080");

    PingControllerApi apiInstance = new PingControllerApi(defaultClient);
    try {
      String result = apiInstance.pong();
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling PingControllerApi#pong");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

**String**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |

