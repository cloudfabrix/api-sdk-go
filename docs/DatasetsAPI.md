# \DatasetsAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**AddDataset**](DatasetsAPI.md#AddDataset) | **Post** /api/v2/datasets | Add a dataset
[**DeleteDataset**](DatasetsAPI.md#DeleteDataset) | **Delete** /api/v2/datasets/dataset/{name} | Delete a dataset
[**DeleteDatasetAllData**](DatasetsAPI.md#DeleteDatasetAllData) | **Delete** /api/v2/datasets/dataset/{name}/data/all | Delete enitre data of a dataset
[**DeleteDatasetRows**](DatasetsAPI.md#DeleteDatasetRows) | **Delete** /api/v2/datasets/dataset/{name}/data | Delete matching dataset rows
[**GetDatasetData**](DatasetsAPI.md#GetDatasetData) | **Get** /api/v2/datasets/dataset/{name}/data | Get data of a dataset
[**GetDatasets**](DatasetsAPI.md#GetDatasets) | **Get** /api/v2/datasets | Fetch meta data about datasets
[**UpdateDatasetData**](DatasetsAPI.md#UpdateDatasetData) | **Put** /api/v2/datasets/dataset/{name}/data | Update rows of a dataset



## AddDataset

> interface{} AddDataset(ctx).DatasetAddModel(datasetAddModel).Execute()

Add a dataset



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
    datasetAddModel := *openapiclient.NewDatasetAddModel("Name_example") // DatasetAddModel | 

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.DatasetsAPI.AddDataset(context.Background()).DatasetAddModel(datasetAddModel).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `DatasetsAPI.AddDataset``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `AddDataset`: interface{}
    fmt.Fprintf(os.Stdout, "Response from `DatasetsAPI.AddDataset`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiAddDatasetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **datasetAddModel** | [**DatasetAddModel**](DatasetAddModel.md) |  | 

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


## DeleteDataset

> interface{} DeleteDataset(ctx, name).Execute()

Delete a dataset



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
    name := "name_example" // string | Dataset name to be deleted.

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.DatasetsAPI.DeleteDataset(context.Background(), name).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `DatasetsAPI.DeleteDataset``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `DeleteDataset`: interface{}
    fmt.Fprintf(os.Stdout, "Response from `DatasetsAPI.DeleteDataset`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**name** | **string** | Dataset name to be deleted. | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteDatasetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


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


## DeleteDatasetAllData

> interface{} DeleteDatasetAllData(ctx, name).Execute()

Delete enitre data of a dataset



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
    name := "name_example" // string | Name of the dataset

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.DatasetsAPI.DeleteDatasetAllData(context.Background(), name).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `DatasetsAPI.DeleteDatasetAllData``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `DeleteDatasetAllData`: interface{}
    fmt.Fprintf(os.Stdout, "Response from `DatasetsAPI.DeleteDatasetAllData`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**name** | **string** | Name of the dataset | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteDatasetAllDataRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


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


## DeleteDatasetRows

> interface{} DeleteDatasetRows(ctx, name).Keys(keys).RequestBody(requestBody).Execute()

Delete matching dataset rows



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
    name := "name_example" // string | Name of the dataset
    keys := []string{"Inner_example"} // []string | Array of keys to match for updating rows
    requestBody := []map[string]interface{}{map[string]interface{}(123)} // []map[string]interface{} | 

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.DatasetsAPI.DeleteDatasetRows(context.Background(), name).Keys(keys).RequestBody(requestBody).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `DatasetsAPI.DeleteDatasetRows``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `DeleteDatasetRows`: interface{}
    fmt.Fprintf(os.Stdout, "Response from `DatasetsAPI.DeleteDatasetRows`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**name** | **string** | Name of the dataset | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteDatasetRowsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **keys** | **[]string** | Array of keys to match for updating rows | 
 **requestBody** | **[]map[string]interface{}** |  | 

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


## GetDatasetData

> TableReportResponse GetDatasetData(ctx, name).CfxqlQuery(cfxqlQuery).Search(search).Sort(sort).Offset(offset).Limit(limit).Execute()

Get data of a dataset



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
    name := "name_example" // string | Name of the dataset
    cfxqlQuery := "cfxqlQuery_example" // string | <a href='https://bot-docs.cloudfabrix.io/reference_guides/cfxql/'>cfxql query</a> string to filter the results (optional)
    search := "search_example" // string | search across fields: ['name'] (optional)
    sort := []string{"Inner_example"} // []string | Sort the output based on given fields. Prepend '-' to sort descending (optional)
    offset := int32(56) // int32 | Offset to start the results from. (optional) (default to 0)
    limit := int32(56) // int32 | Maximum number of results to return (optional) (default to 100)

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.DatasetsAPI.GetDatasetData(context.Background(), name).CfxqlQuery(cfxqlQuery).Search(search).Sort(sort).Offset(offset).Limit(limit).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `DatasetsAPI.GetDatasetData``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `GetDatasetData`: TableReportResponse
    fmt.Fprintf(os.Stdout, "Response from `DatasetsAPI.GetDatasetData`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**name** | **string** | Name of the dataset | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetDatasetDataRequest struct via the builder pattern


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


## GetDatasets

> TableReportResponse GetDatasets(ctx).CfxqlQuery(cfxqlQuery).Search(search).Offset(offset).Limit(limit).Sort(sort).Execute()

Fetch meta data about datasets



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
    search := "search_example" // string | search across fields: ['name', 'schema'] (optional)
    offset := int32(56) // int32 | Offset to start the results from. (optional) (default to 0)
    limit := int32(56) // int32 | Maximum number of results to return (optional) (default to 100)
    sort := []openapiclient.DatasetsEnum{openapiclient.datasets_enum("folder")} // []DatasetsEnum | Sort the output based on given fields (optional) (default to ["-timestamp"])

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.DatasetsAPI.GetDatasets(context.Background()).CfxqlQuery(cfxqlQuery).Search(search).Offset(offset).Limit(limit).Sort(sort).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `DatasetsAPI.GetDatasets``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `GetDatasets`: TableReportResponse
    fmt.Fprintf(os.Stdout, "Response from `DatasetsAPI.GetDatasets`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGetDatasetsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **cfxqlQuery** | **string** | &lt;a href&#x3D;&#39;https://bot-docs.cloudfabrix.io/reference_guides/cfxql/&#39;&gt;cfxql query&lt;/a&gt; string to filter the results | 
 **search** | **string** | search across fields: [&#39;name&#39;, &#39;schema&#39;] | 
 **offset** | **int32** | Offset to start the results from. | [default to 0]
 **limit** | **int32** | Maximum number of results to return | [default to 100]
 **sort** | [**[]DatasetsEnum**](DatasetsEnum.md) | Sort the output based on given fields | [default to [&quot;-timestamp&quot;]]

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


## UpdateDatasetData

> interface{} UpdateDatasetData(ctx, name).RequestBody(requestBody).Replace(replace).Keys(keys).Execute()

Update rows of a dataset



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
    name := "name_example" // string | Name of the dataset
    requestBody := []map[string]interface{}{map[string]interface{}(123)} // []map[string]interface{} | 
    replace := true // bool | If set to true, replace the existing data with new data (optional) (default to false)
    keys := []string{"Inner_example"} // []string | Array of keys to match for updating rows (optional)

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.DatasetsAPI.UpdateDatasetData(context.Background(), name).RequestBody(requestBody).Replace(replace).Keys(keys).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `DatasetsAPI.UpdateDatasetData``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `UpdateDatasetData`: interface{}
    fmt.Fprintf(os.Stdout, "Response from `DatasetsAPI.UpdateDatasetData`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**name** | **string** | Name of the dataset | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateDatasetDataRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **requestBody** | **[]map[string]interface{}** |  | 
 **replace** | **bool** | If set to true, replace the existing data with new data | [default to false]
 **keys** | **[]string** | Array of keys to match for updating rows | 

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

