# spring-testing-client

OpenAPI definition
- API version: v0
  - Build date: 2023-12-04T14:08:19.378694046Z[Etc/UTC]

No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)


*Automatically generated by the [OpenAPI Generator](https://openapi-generator.tech)*


## Requirements

Building the API client library requires:
1. Java 1.8+
2. Maven (3.8.3+)/Gradle (7.2+)

## Installation

To install the API client library to your local Maven repository, simply execute:

```shell
mvn clean install
```

To deploy it to a remote Maven repository instead, configure the settings of the repository and execute:

```shell
mvn clean deploy
```

Refer to the [OSSRH Guide](http://central.sonatype.org/pages/ossrh-guide.html) for more information.

### Maven users

Add this dependency to your project's POM:

```xml
<dependency>
  <groupId>net.internalerror</groupId>
  <artifactId>spring-testing-client</artifactId>
  <version>0.0.1-SNAPSHOT</version>
  <scope>compile</scope>
</dependency>
```

### Gradle users

Add this dependency to your project's build file:

```groovy
  repositories {
    mavenCentral()     // Needed if the 'spring-testing-client' jar has been published to maven central.
    mavenLocal()       // Needed if the 'spring-testing-client' jar has been published to the local maven repo.
  }

  dependencies {
     implementation "net.internalerror:spring-testing-client:0.0.1-SNAPSHOT"
  }
```

### Others

At first generate the JAR by executing:

```shell
mvn clean package
```

Then manually install the following JARs:

* `target/spring-testing-client-0.0.1-SNAPSHOT.jar`
* `target/lib/*.jar`

## Getting Started

Please follow the [installation](#installation) instruction and execute the following Java code:

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

## Documentation for API Endpoints

All URIs are relative to *http://localhost:8080*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*PingControllerApi* | [**ping**](docs/PingControllerApi.md#ping) | **GET** /api/ping | 
*PingControllerApi* | [**pong**](docs/PingControllerApi.md#pong) | **GET** /api/pong | 


## Documentation for Models



<a id="documentation-for-authorization"></a>
## Documentation for Authorization

Endpoints do not require authorization.


## Recommendation

It's recommended to create an instance of `ApiClient` per thread in a multithreaded environment to avoid any potential issues.

## Author



