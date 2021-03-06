---
layout: default
title: Create Zone Category
parent: Zone
grand_parent: Grids
has_children: true
nav_order: 1
---


### 4. Create Zone Category


Op name: 

> scgrids.createZoneCategory

This creates a new Zone category at system level


***Endpoint:***

```bash
Method: POST
Type: application/json
URL: /v1/actions
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Authorization | {{access_token}} | (Required) The Acccess Token or HMAC Signature |
| x-sc-identity | external | (Required) |



***Query params:***

| Key | Value | Description |
| --- | ------|-------------|
| op | scgrids.createZoneCategory | (Required) Operation Name |
| org | {{org}} | (Required) Organisation ID |
| pid | scnoop | (Required) Project ID |



***Body:***

```js        
{
    "Name": "Labs_2",
    "CategoryID": "LABS_2",
    "PropertyTypeID": "SCHOOL"
}
```



***More example Requests/Responses:***


##### I. Example Request: Create Zone Category

***Body:***

```js        
{
    "Name": "Labs",
    "CategoryID": "LABS",
    "PropertyTypeID": "SCHOOL"
}
```

##### I. Example Response: Create Zone Category
```js
{
    "status": 201,
    "message": "Success",
    "data": {
        "Name": "Labs",
        "PropertyTypeID": "SCHOOL",
        "CategoryID": "LABS"
    }
}
```


***Status Code:*** 201

***Error codes:***

##### 400

##### Possible reasons:

###### 1. Missing op/org/pid

###### 2. Invalid characters/improper input body

###### 3. Missing access_token in the header

###### 4. Missing Name/CategoryID/PropertyTypeID

<br>
