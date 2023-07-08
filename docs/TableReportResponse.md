# TableReportResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**LastSortResults** | Pointer to **[]string** | Last sort tags used for internal puposes | [optional] 
**ReportMetaData** | Pointer to **map[string]interface{}** | Meta information about the report, including columns and types etc | [optional] 
**Offset** | Pointer to **int32** | Starting offset in the filtered results | [optional] 
**Limit** | Pointer to **int32** | Maximum number of results to be returned per page | [optional] 
**Sort** | Pointer to **[]string** | Sort order passed as part of request | [optional] 
**TotalCount** | Pointer to **int32** | Total number of results that matched the query | [optional] 
**NumItems** | Pointer to **int32** | Number of results returned in this page | [optional] 
**IsFirst** | Pointer to **bool** | True if this page is first page | [optional] [default to true]
**IsLast** | Pointer to **bool** | True if this page is last page | [optional] [default to true]

## Methods

### NewTableReportResponse

`func NewTableReportResponse() *TableReportResponse`

NewTableReportResponse instantiates a new TableReportResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewTableReportResponseWithDefaults

`func NewTableReportResponseWithDefaults() *TableReportResponse`

NewTableReportResponseWithDefaults instantiates a new TableReportResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetLastSortResults

`func (o *TableReportResponse) GetLastSortResults() []string`

GetLastSortResults returns the LastSortResults field if non-nil, zero value otherwise.

### GetLastSortResultsOk

`func (o *TableReportResponse) GetLastSortResultsOk() (*[]string, bool)`

GetLastSortResultsOk returns a tuple with the LastSortResults field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastSortResults

`func (o *TableReportResponse) SetLastSortResults(v []string)`

SetLastSortResults sets LastSortResults field to given value.

### HasLastSortResults

`func (o *TableReportResponse) HasLastSortResults() bool`

HasLastSortResults returns a boolean if a field has been set.

### GetReportMetaData

`func (o *TableReportResponse) GetReportMetaData() map[string]interface{}`

GetReportMetaData returns the ReportMetaData field if non-nil, zero value otherwise.

### GetReportMetaDataOk

`func (o *TableReportResponse) GetReportMetaDataOk() (*map[string]interface{}, bool)`

GetReportMetaDataOk returns a tuple with the ReportMetaData field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReportMetaData

`func (o *TableReportResponse) SetReportMetaData(v map[string]interface{})`

SetReportMetaData sets ReportMetaData field to given value.

### HasReportMetaData

`func (o *TableReportResponse) HasReportMetaData() bool`

HasReportMetaData returns a boolean if a field has been set.

### GetOffset

`func (o *TableReportResponse) GetOffset() int32`

GetOffset returns the Offset field if non-nil, zero value otherwise.

### GetOffsetOk

`func (o *TableReportResponse) GetOffsetOk() (*int32, bool)`

GetOffsetOk returns a tuple with the Offset field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOffset

`func (o *TableReportResponse) SetOffset(v int32)`

SetOffset sets Offset field to given value.

### HasOffset

`func (o *TableReportResponse) HasOffset() bool`

HasOffset returns a boolean if a field has been set.

### GetLimit

`func (o *TableReportResponse) GetLimit() int32`

GetLimit returns the Limit field if non-nil, zero value otherwise.

### GetLimitOk

`func (o *TableReportResponse) GetLimitOk() (*int32, bool)`

GetLimitOk returns a tuple with the Limit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLimit

`func (o *TableReportResponse) SetLimit(v int32)`

SetLimit sets Limit field to given value.

### HasLimit

`func (o *TableReportResponse) HasLimit() bool`

HasLimit returns a boolean if a field has been set.

### GetSort

`func (o *TableReportResponse) GetSort() []string`

GetSort returns the Sort field if non-nil, zero value otherwise.

### GetSortOk

`func (o *TableReportResponse) GetSortOk() (*[]string, bool)`

GetSortOk returns a tuple with the Sort field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSort

`func (o *TableReportResponse) SetSort(v []string)`

SetSort sets Sort field to given value.

### HasSort

`func (o *TableReportResponse) HasSort() bool`

HasSort returns a boolean if a field has been set.

### GetTotalCount

`func (o *TableReportResponse) GetTotalCount() int32`

GetTotalCount returns the TotalCount field if non-nil, zero value otherwise.

### GetTotalCountOk

`func (o *TableReportResponse) GetTotalCountOk() (*int32, bool)`

GetTotalCountOk returns a tuple with the TotalCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalCount

`func (o *TableReportResponse) SetTotalCount(v int32)`

SetTotalCount sets TotalCount field to given value.

### HasTotalCount

`func (o *TableReportResponse) HasTotalCount() bool`

HasTotalCount returns a boolean if a field has been set.

### GetNumItems

`func (o *TableReportResponse) GetNumItems() int32`

GetNumItems returns the NumItems field if non-nil, zero value otherwise.

### GetNumItemsOk

`func (o *TableReportResponse) GetNumItemsOk() (*int32, bool)`

GetNumItemsOk returns a tuple with the NumItems field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNumItems

`func (o *TableReportResponse) SetNumItems(v int32)`

SetNumItems sets NumItems field to given value.

### HasNumItems

`func (o *TableReportResponse) HasNumItems() bool`

HasNumItems returns a boolean if a field has been set.

### GetIsFirst

`func (o *TableReportResponse) GetIsFirst() bool`

GetIsFirst returns the IsFirst field if non-nil, zero value otherwise.

### GetIsFirstOk

`func (o *TableReportResponse) GetIsFirstOk() (*bool, bool)`

GetIsFirstOk returns a tuple with the IsFirst field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsFirst

`func (o *TableReportResponse) SetIsFirst(v bool)`

SetIsFirst sets IsFirst field to given value.

### HasIsFirst

`func (o *TableReportResponse) HasIsFirst() bool`

HasIsFirst returns a boolean if a field has been set.

### GetIsLast

`func (o *TableReportResponse) GetIsLast() bool`

GetIsLast returns the IsLast field if non-nil, zero value otherwise.

### GetIsLastOk

`func (o *TableReportResponse) GetIsLastOk() (*bool, bool)`

GetIsLastOk returns a tuple with the IsLast field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsLast

`func (o *TableReportResponse) SetIsLast(v bool)`

SetIsLast sets IsLast field to given value.

### HasIsLast

`func (o *TableReportResponse) HasIsLast() bool`

HasIsLast returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


