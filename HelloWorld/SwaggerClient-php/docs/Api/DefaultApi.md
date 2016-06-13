# Swagger\Client\DefaultApi

All URIs are relative to *https://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**helloListGet**](DefaultApi.md#helloListGet) | **GET** /hello/list | 
[**helloUserTimeOfDayGet**](DefaultApi.md#helloUserTimeOfDayGet) | **GET** /hello/{user}/{timeOfDay} | 


# **helloListGet**
> string[] helloListGet()



Returns a list of greetings.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();

try {
    $result = $api_instance->helloListGet();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->helloListGet: ', $e->getMessage(), "\n";
}
?>
```

### Parameters
This endpoint does not need any parameter.

### Return type

**string[]**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **helloUserTimeOfDayGet**
> string helloUserTimeOfDayGet($user, $time_of_day)



Returns a greeting to the user!

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$user = "user_example"; // string | The name of the user to greet.
$time_of_day = "time_of_day_example"; // string | The time of the day (morning, afternoon, evening, night)

try {
    $result = $api_instance->helloUserTimeOfDayGet($user, $time_of_day);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->helloUserTimeOfDayGet: ', $e->getMessage(), "\n";
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user** | **string**| The name of the user to greet. | 
 **time_of_day** | **string**| The time of the day (morning, afternoon, evening, night) | 

### Return type

**string**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

