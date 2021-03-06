---
layout: default
title: Building to Zone Map
parent: Building
grand_parent: Grids
has_children: true
nav_order: 1
---


### 2. Building Zone Map


Op Name: 

> scgrids.buildingZoneMap

This lists a given Building's zone name and zone id map


***Endpoint:***

```bash
Method: POST
Type: application/json
URL: /v1/actions
```

***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Authorization | {{access_tokren}} | (Required) The Acccess Token or HMAC Signature |
| x-sc-identity | external | (Required) |



***Query params:***

| Key | Value | Description |
| --- | ------|-------------|
| op | scgrids.buildingZoneMap | (Required) Operation Name |
| org | {{org}} | (Required) Organisation Name |
| pid | {{pid}} | (Required) Project ID |



***Body:***

```js        
{
    "ESK": "{{ESK}}"
}
```

***Error codes:***

##### 400

##### Possible reasons:

###### 1. Missing op, org or pid
###### 2. Invalid characters/improper input body
