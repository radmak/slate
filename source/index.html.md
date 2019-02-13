# Introduction

Welcome to People API! You can use our API to access People API endpoints and get personal information of people from our database.

# Authentication

This is a public API and does not require any API key for authentication.

# People

## GetAll

Returns an array of personal information of all people.

> JSON:

```json
[  
  {
    "Id": 1,
    "Name": "Mahesh",
    "Occupation": "IT",
    "Contact": 9876543210,
    "Address": "Paud Road, Pune",
    "Guid": null,
    "UDID": "0e3f9a93-7f29-4d2a-a371-d30c019c8667",
    "APKversion": "1.2"
  }  
]
```
### Query Parameters

This endpoint does not require any query parameters.

## GetPeople

Retrieves personal information of a specific person.

### Request

Key | Value
--------- | -----------
Id | <b>integer.</b> The ID of the person whose information is to be retrieved.

> JSON:

```json
{
  "Id": 1  
}
```
### Response

Key | Value
--------- | -----------
Id | <b>long.</b> The ID of this person.
Name | <b>string.</b> The name of this person.
Occupation | <b>string.</b> The occupation of this person.
Contact | <b>string.</b> The contact details of this person, generally a mobile number.
Address | <b>string.</b> The Address of this person.
Guid | <b>string.</b> A globally unique identifier of the application installed on the machine of this person.
UDID | <b>string.</b> A unique identifier of the device of this person.
APKversion | <b>string.</b> The version of the software installed on the device of this person.

> JSON:

```json
  {
    "Id": 1,
    "Name": "Mahesh",
    "Occupation": "IT",
    "Contact": "9876543210",
    "Address": "Paud Road, Pune",
    "Guid": null,
    "UDID": "0e3f9a93-7f29-4d2a-a371-d30c019c8667",
    "APKversion": "1.2"
  }
```







