# \DashboardsAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GetDashboards**](DashboardsAPI.md#GetDashboards) | **Get** /api/v2/dashboards | Fetch meta data for dashboards



## GetDashboards

> TableReportResponse GetDashboards(ctx).CfxqlQuery(cfxqlQuery).Search(search).Offset(offset).Limit(limit).Sort(sort).Execute()

Fetch meta data for dashboards



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
    search := "search_example" // string | search across fields: ['name', 'description', 'usecase', 'category', 'version'] (optional)
    offset := int32(56) // int32 | Offset to start the results from. (optional) (default to 0)
    limit := int32(56) // int32 | Maximum number of results to return (optional) (default to 100)
    sort := []openapiclient.DashboardsEnum{openapiclient.dashboards_enum("category")} // []DashboardsEnum | Sort the output based on given fields (optional) (default to ["-timestamp"])

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.DashboardsAPI.GetDashboards(context.Background()).CfxqlQuery(cfxqlQuery).Search(search).Offset(offset).Limit(limit).Sort(sort).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `DashboardsAPI.GetDashboards``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `GetDashboards`: TableReportResponse
    fmt.Fprintf(os.Stdout, "Response from `DashboardsAPI.GetDashboards`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGetDashboardsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **cfxqlQuery** | **string** | &lt;a href&#x3D;&#39;https://bot-docs.cloudfabrix.io/reference_guides/cfxql/&#39;&gt;cfxql query&lt;/a&gt; string to filter the results | 
 **search** | **string** | search across fields: [&#39;name&#39;, &#39;description&#39;, &#39;usecase&#39;, &#39;category&#39;, &#39;version&#39;] | 
 **offset** | **int32** | Offset to start the results from. | [default to 0]
 **limit** | **int32** | Maximum number of results to return | [default to 100]
 **sort** | [**[]DashboardsEnum**](DashboardsEnum.md) | Sort the output based on given fields | [default to [&quot;-timestamp&quot;]]

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

