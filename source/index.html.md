# Introduction

Welcome to People API! You can use this API to access People API endpoints and get information of people from our database.

# Authentication

This is a public API and does not require any API key for authentication.

# People

## GetAll

Returns an array of information of all people.

### Request

There is no payload for a <b> GetAll </b> request.

### Response

> JSON:

```json
[  
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
]
```

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

## GetPeople

Retrieves information of a specific person.

### Request

> JSON:

```json
{
  "Id": 1  
}
```

Key | Value
--------- | -----------
Id | <b>integer.</b> The ID of the person whose information is to be retrieved.

### Response

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








