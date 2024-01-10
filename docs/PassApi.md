# PassApi

All URIs are relative to **

Method | HTTP request | Description
------------- | ------------- | -------------
[**createOrUpdatePass**](PassApi.md#createOrUpdatePass) | **POST** /pass | This method creates or (if the pass id already exists) updates a pass, so you don&#39;t have to track ids and creation status of your passes.
[**deletePass**](PassApi.md#deletePass) | **DELETE** /pass | Delete pass by pass id.
[**getPass**](PassApi.md#getPass) | **GET** /pass | Get pass information by pass id.
[**passList**](PassApi.md#passList) | **GET** /pass/list | Retrieve the list of active pass ids for a given pass type.
[**passSync**](PassApi.md#passSync) | **POST** /pass/sync | Send updates to all active passes for a given pass type.


## **createOrUpdatePass**

This method creates or (if the pass id already exists) updates a pass, so you don't have to track ids and creation status of your passes.

This method creates or (if the pass id already exists) updates a pass, so you don't have to track ids and creation status of your passes.

### Example
```bash
 createOrUpdatePass  passTypeId=value  passId=value
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **passTypeId** | [**map**](.md) | your pass type id, for example P963493 (Urban Fitness) |
 **passId** | [**map**](.md) | id of the pass (provided by you when creating the pass or automatically set by passmeister) | [optional]

### Return type

(empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not Applicable
 - **Accept**: Not Applicable

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

## **deletePass**

Delete pass by pass id.

Delete pass by pass id.

### Example
```bash
 deletePass  passTypeId=value  passId=value
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **passTypeId** | [**map**](.md) | your pass type id, for example P963493 (Urban Fitness) |
 **passId** | [**map**](.md) | id of the pass |

### Return type

(empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not Applicable
 - **Accept**: Not Applicable

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

## **getPass**

Get pass information by pass id.

Get pass information by pass id.

### Example
```bash
 getPass  passTypeId=value  passId=value
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **passTypeId** | [**map**](.md) | your pass type id, for example P963493 (Urban Fitness) |
 **passId** | [**map**](.md) | id of the pass |

### Return type

(empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not Applicable
 - **Accept**: Not Applicable

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

## **passList**

Retrieve the list of active pass ids for a given pass type.

Retrieve the list of active pass ids for a given pass type.

### Example
```bash
 passList  passTypeId=value  page=value  limit=value
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **passTypeId** | [**map**](.md) | your pass type id, for example P963493 (Urban Fitness) |
 **page** | [**map**](.md) |  | [optional]
 **limit** | [**map**](.md) |  | [optional]

### Return type

(empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not Applicable
 - **Accept**: Not Applicable

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

## **passSync**

Send updates to all active passes for a given pass type.

For example: you changed the pass type layout and now you want to update all installed passes. (The API call only confirms the scheduling of the updates, actual updating of passes on your customers devices can take a while.)

### Example
```bash
 passSync  passTypeId=value
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **passTypeId** | [**map**](.md) | your pass type id, for example P963493 (Urban Fitness) |

### Return type

(empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not Applicable
 - **Accept**: Not Applicable

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

