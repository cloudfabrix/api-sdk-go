# UserDetails

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Authenticated** | Pointer to **bool** | Whether user is authenticated | [optional] 
**Company** | Pointer to **string** | Company the user belongs to | [optional] 
**FirstName** | Pointer to **string** | First name | [optional] 
**Id** | Pointer to **string** | Id of the user (email address) | [optional] 
**IsAuthenticated** | Pointer to **bool** | Alias to &#39;authenticated&#39; | [optional] 
**IsWorkspaceadmin** | Pointer to **bool** | Is the user a workspace admin | [optional] 
**IsWorkspacecreator** | Pointer to **bool** | Is the user a workspace creator | [optional] 
**LastName** | Pointer to **bool** | Last Name | [optional] 
**Lastname** | Pointer to **bool** | Alias to last_name | [optional] 
**LoginTime** | Pointer to **string** | Login time in ISO format | [optional] 
**RdacAuthToken** | Pointer to **string** | Authentication Token | [optional] 
**RemoteUser** | Pointer to **bool** | Whether user is a remote user or a local user | [optional] 
**Role** | Pointer to **string** | User Role | [optional] 
**SessionId** | Pointer to **string** | Current session id | [optional] 
**Status** | Pointer to **string** | Current status of the user | [optional] 
**Tenantid** | Pointer to **string** | Tenant ID of the user | [optional] 
**User** | Pointer to **string** | alias to &#39;id&#39; | [optional] 
**Workspace** | Pointer to **string** | Name of the workspace | [optional] 
**Workspaceid** | Pointer to **string** | ID of the workspace | [optional] 

## Methods

### NewUserDetails

`func NewUserDetails() *UserDetails`

NewUserDetails instantiates a new UserDetails object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUserDetailsWithDefaults

`func NewUserDetailsWithDefaults() *UserDetails`

NewUserDetailsWithDefaults instantiates a new UserDetails object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAuthenticated

`func (o *UserDetails) GetAuthenticated() bool`

GetAuthenticated returns the Authenticated field if non-nil, zero value otherwise.

### GetAuthenticatedOk

`func (o *UserDetails) GetAuthenticatedOk() (*bool, bool)`

GetAuthenticatedOk returns a tuple with the Authenticated field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAuthenticated

`func (o *UserDetails) SetAuthenticated(v bool)`

SetAuthenticated sets Authenticated field to given value.

### HasAuthenticated

`func (o *UserDetails) HasAuthenticated() bool`

HasAuthenticated returns a boolean if a field has been set.

### GetCompany

`func (o *UserDetails) GetCompany() string`

GetCompany returns the Company field if non-nil, zero value otherwise.

### GetCompanyOk

`func (o *UserDetails) GetCompanyOk() (*string, bool)`

GetCompanyOk returns a tuple with the Company field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCompany

`func (o *UserDetails) SetCompany(v string)`

SetCompany sets Company field to given value.

### HasCompany

`func (o *UserDetails) HasCompany() bool`

HasCompany returns a boolean if a field has been set.

### GetFirstName

`func (o *UserDetails) GetFirstName() string`

GetFirstName returns the FirstName field if non-nil, zero value otherwise.

### GetFirstNameOk

`func (o *UserDetails) GetFirstNameOk() (*string, bool)`

GetFirstNameOk returns a tuple with the FirstName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFirstName

`func (o *UserDetails) SetFirstName(v string)`

SetFirstName sets FirstName field to given value.

### HasFirstName

`func (o *UserDetails) HasFirstName() bool`

HasFirstName returns a boolean if a field has been set.

### GetId

`func (o *UserDetails) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *UserDetails) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *UserDetails) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *UserDetails) HasId() bool`

HasId returns a boolean if a field has been set.

### GetIsAuthenticated

`func (o *UserDetails) GetIsAuthenticated() bool`

GetIsAuthenticated returns the IsAuthenticated field if non-nil, zero value otherwise.

### GetIsAuthenticatedOk

`func (o *UserDetails) GetIsAuthenticatedOk() (*bool, bool)`

GetIsAuthenticatedOk returns a tuple with the IsAuthenticated field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsAuthenticated

`func (o *UserDetails) SetIsAuthenticated(v bool)`

SetIsAuthenticated sets IsAuthenticated field to given value.

### HasIsAuthenticated

`func (o *UserDetails) HasIsAuthenticated() bool`

HasIsAuthenticated returns a boolean if a field has been set.

### GetIsWorkspaceadmin

`func (o *UserDetails) GetIsWorkspaceadmin() bool`

GetIsWorkspaceadmin returns the IsWorkspaceadmin field if non-nil, zero value otherwise.

### GetIsWorkspaceadminOk

`func (o *UserDetails) GetIsWorkspaceadminOk() (*bool, bool)`

GetIsWorkspaceadminOk returns a tuple with the IsWorkspaceadmin field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsWorkspaceadmin

`func (o *UserDetails) SetIsWorkspaceadmin(v bool)`

SetIsWorkspaceadmin sets IsWorkspaceadmin field to given value.

### HasIsWorkspaceadmin

`func (o *UserDetails) HasIsWorkspaceadmin() bool`

HasIsWorkspaceadmin returns a boolean if a field has been set.

### GetIsWorkspacecreator

`func (o *UserDetails) GetIsWorkspacecreator() bool`

GetIsWorkspacecreator returns the IsWorkspacecreator field if non-nil, zero value otherwise.

### GetIsWorkspacecreatorOk

`func (o *UserDetails) GetIsWorkspacecreatorOk() (*bool, bool)`

GetIsWorkspacecreatorOk returns a tuple with the IsWorkspacecreator field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsWorkspacecreator

`func (o *UserDetails) SetIsWorkspacecreator(v bool)`

SetIsWorkspacecreator sets IsWorkspacecreator field to given value.

### HasIsWorkspacecreator

`func (o *UserDetails) HasIsWorkspacecreator() bool`

HasIsWorkspacecreator returns a boolean if a field has been set.

### GetLastName

`func (o *UserDetails) GetLastName() bool`

GetLastName returns the LastName field if non-nil, zero value otherwise.

### GetLastNameOk

`func (o *UserDetails) GetLastNameOk() (*bool, bool)`

GetLastNameOk returns a tuple with the LastName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastName

`func (o *UserDetails) SetLastName(v bool)`

SetLastName sets LastName field to given value.

### HasLastName

`func (o *UserDetails) HasLastName() bool`

HasLastName returns a boolean if a field has been set.

### GetLastname

`func (o *UserDetails) GetLastname() bool`

GetLastname returns the Lastname field if non-nil, zero value otherwise.

### GetLastnameOk

`func (o *UserDetails) GetLastnameOk() (*bool, bool)`

GetLastnameOk returns a tuple with the Lastname field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastname

`func (o *UserDetails) SetLastname(v bool)`

SetLastname sets Lastname field to given value.

### HasLastname

`func (o *UserDetails) HasLastname() bool`

HasLastname returns a boolean if a field has been set.

### GetLoginTime

`func (o *UserDetails) GetLoginTime() string`

GetLoginTime returns the LoginTime field if non-nil, zero value otherwise.

### GetLoginTimeOk

`func (o *UserDetails) GetLoginTimeOk() (*string, bool)`

GetLoginTimeOk returns a tuple with the LoginTime field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLoginTime

`func (o *UserDetails) SetLoginTime(v string)`

SetLoginTime sets LoginTime field to given value.

### HasLoginTime

`func (o *UserDetails) HasLoginTime() bool`

HasLoginTime returns a boolean if a field has been set.

### GetRdacAuthToken

`func (o *UserDetails) GetRdacAuthToken() string`

GetRdacAuthToken returns the RdacAuthToken field if non-nil, zero value otherwise.

### GetRdacAuthTokenOk

`func (o *UserDetails) GetRdacAuthTokenOk() (*string, bool)`

GetRdacAuthTokenOk returns a tuple with the RdacAuthToken field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRdacAuthToken

`func (o *UserDetails) SetRdacAuthToken(v string)`

SetRdacAuthToken sets RdacAuthToken field to given value.

### HasRdacAuthToken

`func (o *UserDetails) HasRdacAuthToken() bool`

HasRdacAuthToken returns a boolean if a field has been set.

### GetRemoteUser

`func (o *UserDetails) GetRemoteUser() bool`

GetRemoteUser returns the RemoteUser field if non-nil, zero value otherwise.

### GetRemoteUserOk

`func (o *UserDetails) GetRemoteUserOk() (*bool, bool)`

GetRemoteUserOk returns a tuple with the RemoteUser field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRemoteUser

`func (o *UserDetails) SetRemoteUser(v bool)`

SetRemoteUser sets RemoteUser field to given value.

### HasRemoteUser

`func (o *UserDetails) HasRemoteUser() bool`

HasRemoteUser returns a boolean if a field has been set.

### GetRole

`func (o *UserDetails) GetRole() string`

GetRole returns the Role field if non-nil, zero value otherwise.

### GetRoleOk

`func (o *UserDetails) GetRoleOk() (*string, bool)`

GetRoleOk returns a tuple with the Role field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRole

`func (o *UserDetails) SetRole(v string)`

SetRole sets Role field to given value.

### HasRole

`func (o *UserDetails) HasRole() bool`

HasRole returns a boolean if a field has been set.

### GetSessionId

`func (o *UserDetails) GetSessionId() string`

GetSessionId returns the SessionId field if non-nil, zero value otherwise.

### GetSessionIdOk

`func (o *UserDetails) GetSessionIdOk() (*string, bool)`

GetSessionIdOk returns a tuple with the SessionId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSessionId

`func (o *UserDetails) SetSessionId(v string)`

SetSessionId sets SessionId field to given value.

### HasSessionId

`func (o *UserDetails) HasSessionId() bool`

HasSessionId returns a boolean if a field has been set.

### GetStatus

`func (o *UserDetails) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *UserDetails) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *UserDetails) SetStatus(v string)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *UserDetails) HasStatus() bool`

HasStatus returns a boolean if a field has been set.

### GetTenantid

`func (o *UserDetails) GetTenantid() string`

GetTenantid returns the Tenantid field if non-nil, zero value otherwise.

### GetTenantidOk

`func (o *UserDetails) GetTenantidOk() (*string, bool)`

GetTenantidOk returns a tuple with the Tenantid field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTenantid

`func (o *UserDetails) SetTenantid(v string)`

SetTenantid sets Tenantid field to given value.

### HasTenantid

`func (o *UserDetails) HasTenantid() bool`

HasTenantid returns a boolean if a field has been set.

### GetUser

`func (o *UserDetails) GetUser() string`

GetUser returns the User field if non-nil, zero value otherwise.

### GetUserOk

`func (o *UserDetails) GetUserOk() (*string, bool)`

GetUserOk returns a tuple with the User field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUser

`func (o *UserDetails) SetUser(v string)`

SetUser sets User field to given value.

### HasUser

`func (o *UserDetails) HasUser() bool`

HasUser returns a boolean if a field has been set.

### GetWorkspace

`func (o *UserDetails) GetWorkspace() string`

GetWorkspace returns the Workspace field if non-nil, zero value otherwise.

### GetWorkspaceOk

`func (o *UserDetails) GetWorkspaceOk() (*string, bool)`

GetWorkspaceOk returns a tuple with the Workspace field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWorkspace

`func (o *UserDetails) SetWorkspace(v string)`

SetWorkspace sets Workspace field to given value.

### HasWorkspace

`func (o *UserDetails) HasWorkspace() bool`

HasWorkspace returns a boolean if a field has been set.

### GetWorkspaceid

`func (o *UserDetails) GetWorkspaceid() string`

GetWorkspaceid returns the Workspaceid field if non-nil, zero value otherwise.

### GetWorkspaceidOk

`func (o *UserDetails) GetWorkspaceidOk() (*string, bool)`

GetWorkspaceidOk returns a tuple with the Workspaceid field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWorkspaceid

`func (o *UserDetails) SetWorkspaceid(v string)`

SetWorkspaceid sets Workspaceid field to given value.

### HasWorkspaceid

`func (o *UserDetails) HasWorkspaceid() bool`

HasWorkspaceid returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


