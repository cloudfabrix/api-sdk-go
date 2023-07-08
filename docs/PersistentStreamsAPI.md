# \PersistentStreamsAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**AddPstream**](PersistentStreamsAPI.md#AddPstream) | **Post** /api/v2/pstreams | Add a pstream
[**DeletePstream**](PersistentStreamsAPI.md#DeletePstream) | **Delete** /api/v2/pstreams/pstream/{name} | Delete a pstream.
[**EditPstream**](PersistentStreamsAPI.md#EditPstream) | **Put** /api/v2/pstreams/pstream/{name} | Edit attributes of a pstream
[**GetPstreamData**](PersistentStreamsAPI.md#GetPstreamData) | **Get** /api/v2/pstreams/pstream/{name}/data | Get data of a pstream
[**GetPstreams**](PersistentStreamsAPI.md#GetPstreams) | **Get** /api/v2/pstreams | Fetch meta data about pstreams



## AddPstream

> interface{} AddPstream(ctx).PstreamAddModel(pstreamAddModel).Execute()

Add a pstream



### Example

```go
package main

import (
    "context"
    "fmt"
    "os"
    openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
    pstreamAddModel := *openapiclient.NewPstreamAddModel("Name_example") // PstreamAddModel | 

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.PersistentStreamsAPI.AddPstream(context.Background()).PstreamAddModel(pstreamAddModel).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `PersistentStreamsAPI.AddPstream``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `AddPstream`: interface{}
    fmt.Fprintf(os.Stdout, "Response from `PersistentStreamsAPI.AddPstream`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiAddPstreamRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **pstreamAddModel** | [**PstreamAddModel**](PstreamAddModel.md) |  | 

### Return type

**interface{}**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeletePstream

> interface{} DeletePstream(ctx, name).DeleteData(deleteData).Execute()

Delete a pstream.



### Example

```go
package main

import (
    "context"
    "fmt"
    "os"
    openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
    name := "name_example" // string | Name of the pstream to be deleted
    deleteData := true // bool | Delete data as well. If data is not deleted, adding the same pstream again will add the old data back. (optional) (default to false)

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.PersistentStreamsAPI.DeletePstream(context.Background(), name).DeleteData(deleteData).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `PersistentStreamsAPI.DeletePstream``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `DeletePstream`: interface{}
    fmt.Fprintf(os.Stdout, "Response from `PersistentStreamsAPI.DeletePstream`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**name** | **string** | Name of the pstream to be deleted | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeletePstreamRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **deleteData** | **bool** | Delete data as well. If data is not deleted, adding the same pstream again will add the old data back. | [default to false]

### Return type

**interface{}**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## EditPstream

> interface{} EditPstream(ctx, name).PstreamEditModel(pstreamEditModel).Execute()

Edit attributes of a pstream



### Example

```go
package main

import (
    "context"
    "fmt"
    "os"
    openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
    name := "name_example" // string | Name of the pstream to be edited
    pstreamEditModel := *openapiclient.NewPstreamEditModel() // PstreamEditModel | 

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.PersistentStreamsAPI.EditPstream(context.Background(), name).PstreamEditModel(pstreamEditModel).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `PersistentStreamsAPI.EditPstream``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `EditPstream`: interface{}
    fmt.Fprintf(os.Stdout, "Response from `PersistentStreamsAPI.EditPstream`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**name** | **string** | Name of the pstream to be edited | 

### Other Parameters

Other parameters are passed through a pointer to a apiEditPstreamRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **pstreamEditModel** | [**PstreamEditModel**](PstreamEditModel.md) |  | 

### Return type

**interface{}**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetPstreamData

> TableReportResponse GetPstreamData(ctx, name).CfxqlQuery(cfxqlQuery).Search(search).Sort(sort).Offset(offset).Limit(limit).Execute()

Get data of a pstream



### Example

```go
package main

import (
    "context"
    "fmt"
    "os"
    openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
    name := "name_example" // string | Name of the pstream
    cfxqlQuery := "cfxqlQuery_example" // string | <a href='https://bot-docs.cloudfabrix.io/reference_guides/cfxql/'>cfxql query</a> string to filter the results (optional)
    search := "search_example" // string | search across fields: ['name'] (optional)
    sort := []string{"Inner_example"} // []string | Sort the output based on given fields. Prepend '-' to sort descending (optional)
    offset := int32(56) // int32 | Offset to start the results from. (optional) (default to 0)
    limit := int32(56) // int32 | Maximum number of results to return (optional) (default to 100)

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.PersistentStreamsAPI.GetPstreamData(context.Background(), name).CfxqlQuery(cfxqlQuery).Search(search).Sort(sort).Offset(offset).Limit(limit).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `PersistentStreamsAPI.GetPstreamData``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `GetPstreamData`: TableReportResponse
    fmt.Fprintf(os.Stdout, "Response from `PersistentStreamsAPI.GetPstreamData`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**name** | **string** | Name of the pstream | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetPstreamDataRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **cfxqlQuery** | **string** | &lt;a href&#x3D;&#39;https://bot-docs.cloudfabrix.io/reference_guides/cfxql/&#39;&gt;cfxql query&lt;/a&gt; string to filter the results | 
 **search** | **string** | search across fields: [&#39;name&#39;] | 
 **sort** | **[]string** | Sort the output based on given fields. Prepend &#39;-&#39; to sort descending | 
 **offset** | **int32** | Offset to start the results from. | [default to 0]
 **limit** | **int32** | Maximum number of results to return | [default to 100]

### Return type

[**TableReportResponse**](TableReportResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetPstreams

> TableReportResponse GetPstreams(ctx).CfxqlQuery(cfxqlQuery).Search(search).Offset(offset).Limit(limit).Sort(sort).Execute()

Fetch meta data about pstreams



### Example

```go
package main

import (
    "context"
    "fmt"
    "os"
    openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
    cfxqlQuery := "cfxqlQuery_example" // string | <a href='https://bot-docs.cloudfabrix.io/reference_guides/cfxql/'>cfxql query</a> string to filter the results (optional)
    search := "search_example" // string | search across fields: ['name'] (optional)
    offset := int32(56) // int32 | Offset to start the results from. (optional) (default to 0)
    limit := int32(56) // int32 | Maximum number of results to return (optional) (default to 100)
    sort := []openapiclient.PstreamsEnum{openapiclient.pstreams_enum("collection_status")} // []PstreamsEnum | Sort the output based on given fields (optional) (default to ["-timestamp"])

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.PersistentStreamsAPI.GetPstreams(context.Background()).CfxqlQuery(cfxqlQuery).Search(search).Offset(offset).Limit(limit).Sort(sort).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `PersistentStreamsAPI.GetPstreams``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `GetPstreams`: TableReportResponse
    fmt.Fprintf(os.Stdout, "Response from `PersistentStreamsAPI.GetPstreams`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGetPstreamsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **cfxqlQuery** | **string** | &lt;a href&#x3D;&#39;https://bot-docs.cloudfabrix.io/reference_guides/cfxql/&#39;&gt;cfxql query&lt;/a&gt; string to filter the results | 
 **search** | **string** | search across fields: [&#39;name&#39;] | 
 **offset** | **int32** | Offset to start the results from. | [default to 0]
 **limit** | **int32** | Maximum number of results to return | [default to 100]
 **sort** | [**[]PstreamsEnum**](PstreamsEnum.md) | Sort the output based on given fields | [default to [&quot;-timestamp&quot;]]

### Return type

[**TableReportResponse**](TableReportResponse.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

