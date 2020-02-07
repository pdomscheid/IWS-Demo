# Shelter.PetApi

All URIs are relative to *https://virtserver.swaggerhub.com/molatho1/Shelter/1.0.0*

Method | HTTP request | Description
------------- | ------------- | -------------
[**addPet**](PetApi.md#addPet) | **POST** /pet | Add a pet in the shelter
[**deletePet**](PetApi.md#deletePet) | **DELETE** /pet/{petId} | Deletes a pet
[**getPetById**](PetApi.md#getPetById) | **GET** /pet/{petId} | Find pet by ID
[**getPets**](PetApi.md#getPets) | **GET** /pet | Gets all pets
[**updatePet**](PetApi.md#updatePet) | **PUT** /pet/{petId} | Update an existing pet


<a name="addPet"></a>
# **addPet**
> addPet(body)

Add a pet in the shelter

### Example
```javascript
var Shelter = require('shelter');

var apiInstance = new Shelter.PetApi();

var body = new Shelter.Pet(); // Pet | Pet object that needs to be added to the shelter


var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully.');
  }
};
apiInstance.addPet(body, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**Pet**](Pet.md)| Pet object that needs to be added to the shelter | 

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, application/xml

<a name="deletePet"></a>
# **deletePet**
> deletePet(petId, opts)

Deletes a pet

### Example
```javascript
var Shelter = require('shelter');

var apiInstance = new Shelter.PetApi();

var petId = 789; // Number | Pet id to delete

var opts = { 
  'apiKey': "apiKey_example" // String | 
};

var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully.');
  }
};
apiInstance.deletePet(petId, opts, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **petId** | **Number**| Pet id to delete | 
 **apiKey** | **String**|  | [optional] 

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, application/xml

<a name="getPetById"></a>
# **getPetById**
> Pet getPetById(petId)

Find pet by ID

Returns a single pet

### Example
```javascript
var Shelter = require('shelter');

var apiInstance = new Shelter.PetApi();

var petId = 789; // Number | ID of pet that needs to be updated


var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.getPetById(petId, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **petId** | **Number**| ID of pet that needs to be updated | 

### Return type

[**Pet**](Pet.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, application/xml

<a name="getPets"></a>
# **getPets**
> Pet getPets()

Gets all pets

Returns all pets

### Example
```javascript
var Shelter = require('shelter');

var apiInstance = new Shelter.PetApi();

var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
};
apiInstance.getPets(callback);
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**Pet**](Pet.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, application/xml

<a name="updatePet"></a>
# **updatePet**
> updatePet(body, petId)

Update an existing pet

### Example
```javascript
var Shelter = require('shelter');

var apiInstance = new Shelter.PetApi();

var body = new Shelter.Pet(); // Pet | Pet object that needs to be added to the shelter

var petId = 789; // Number | ID of pet that needs to be updated


var callback = function(error, data, response) {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully.');
  }
};
apiInstance.updatePet(body, petId, callback);
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**Pet**](Pet.md)| Pet object that needs to be added to the shelter | 
 **petId** | **Number**| ID of pet that needs to be updated | 

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json, application/xml
 - **Accept**: application/json, application/xml

