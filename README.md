
# Getting Started with APIMATIC Calculator

## Introduction

Simple calculator API hosted on APIMATIC

## Install the Package

Install the SDK by adding the following dependency in your project's pom.xml file:

```xml
<dependency>
  <groupId>io.github.sufyankhanrao</groupId>
  <artifactId>apimatic-calculator-sdk</artifactId>
  <version>2.0.0</version>
</dependency>
```

You can also view the package at:
https://mvnrepository.com/artifact/io.github.sufyankhanrao/apimatic-calculator-sdk/2.0.0

## Test the SDK

The generated code and the server can be tested using automatically generated test cases.
JUnit is used as the testing framework and test runner.

In Eclipse, for running the tests do the following:

1. Select the project APIMATICCalculatorLib from the package explorer.
2. Select `Run -> Run as -> JUnit Test` or use `Alt + Shift + X` followed by `T` to run the Tests.

## Initialize the API Client

**_Note:_** Documentation for the client can be found [here.](https://www.github.com/sufyankhanrao/testing-java-sdk/tree/2.0.0/doc/client.md)

The following parameters are configurable for the API Client:

| Parameter | Type | Description |
|  --- | --- | --- |
| `environment` | Environment | The API environment. <br> **Default: `Environment.PRODUCTION`** |
| `httpClientConfig` | [`ReadonlyHttpClientConfiguration`](https://www.github.com/sufyankhanrao/testing-java-sdk/tree/2.0.0/doc/http-client-configuration.md) | Http Client Configuration instance. |

The API client can be initialized as follows:

```java
APIMATICCalculatorClient client = new APIMATICCalculatorClient.Builder()
    .httpClientConfig(configBuilder -> configBuilder
            .timeout(0))
    .environment(Environment.PRODUCTION)
    .build();
```

## List of APIs

* [Simple Calculator](https://www.github.com/sufyankhanrao/testing-java-sdk/tree/2.0.0/doc/controllers/simple-calculator.md)

## Classes Documentation

* [Utility Classes](https://www.github.com/sufyankhanrao/testing-java-sdk/tree/2.0.0/doc/utility-classes.md)
* [HttpRequest](https://www.github.com/sufyankhanrao/testing-java-sdk/tree/2.0.0/doc/http-request.md)
* [HttpResponse](https://www.github.com/sufyankhanrao/testing-java-sdk/tree/2.0.0/doc/http-response.md)
* [HttpStringResponse](https://www.github.com/sufyankhanrao/testing-java-sdk/tree/2.0.0/doc/http-string-response.md)
* [HttpContext](https://www.github.com/sufyankhanrao/testing-java-sdk/tree/2.0.0/doc/http-context.md)
* [HttpBodyRequest](https://www.github.com/sufyankhanrao/testing-java-sdk/tree/2.0.0/doc/http-body-request.md)
* [HttpCallback Interface](https://www.github.com/sufyankhanrao/testing-java-sdk/tree/2.0.0/doc/http-callback-interface.md)
* [Headers](https://www.github.com/sufyankhanrao/testing-java-sdk/tree/2.0.0/doc/headers.md)
* [ApiException](https://www.github.com/sufyankhanrao/testing-java-sdk/tree/2.0.0/doc/api-exception.md)
* [Configuration Interface](https://www.github.com/sufyankhanrao/testing-java-sdk/tree/2.0.0/doc/configuration-interface.md)
* [HttpClientConfiguration](https://www.github.com/sufyankhanrao/testing-java-sdk/tree/2.0.0/doc/http-client-configuration.md)
* [HttpClientConfiguration.Builder](https://www.github.com/sufyankhanrao/testing-java-sdk/tree/2.0.0/doc/http-client-configuration-builder.md)

