# LoginInput

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**User** | **string** |  | 
**Password** | **string** |  | 

## Methods

### NewLoginInput

`func NewLoginInput(user string, password string, ) *LoginInput`

NewLoginInput instantiates a new LoginInput object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewLoginInputWithDefaults

`func NewLoginInputWithDefaults() *LoginInput`

NewLoginInputWithDefaults instantiates a new LoginInput object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetUser

`func (o *LoginInput) GetUser() string`

GetUser returns the User field if non-nil, zero value otherwise.

### GetUserOk

`func (o *LoginInput) GetUserOk() (*string, bool)`

GetUserOk returns a tuple with the User field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUser

`func (o *LoginInput) SetUser(v string)`

SetUser sets User field to given value.


### GetPassword

`func (o *LoginInput) GetPassword() string`

GetPassword returns the Password field if non-nil, zero value otherwise.

### GetPasswordOk

`func (o *LoginInput) GetPasswordOk() (*string, bool)`

GetPasswordOk returns a tuple with the Password field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPassword

`func (o *LoginInput) SetPassword(v string)`

SetPassword sets Password field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


