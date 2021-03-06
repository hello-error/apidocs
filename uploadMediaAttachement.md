---
layout: default
title: Upload Media Attachement
parent: Miscellaneous
grand_parent: Grids
has_children: true
nav_order: 1
---


### 3. Upload Media Attachment


Op name:

> scgrids.uploadMediaAttachment

This uploads media attachments for a given entity and of a given type


***Endpoint:***

```bash
Method: POST
Type: FORMDATA
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
| op | scgrids.uploadMediaAttachment | (Required) Operation Name |
| org | scnoop | (Required) Organisation Name |
| pid | scnoop | (Required) Project ID |



***Body:***

| Key | Value | Description |
| --- | ------|-------------|
| Type | excel | (Required) Supports image/video |
| Entity | incident | (Required) Supports incident/audits |
| File |  | (Required) File to upload |


***Error codes:***

##### 400

##### Possible reasons:

###### 1. Missing op/org/pid

###### 4. Missing Type/Entity/File in the body

###### 5. If the fileoe Image type Image exceeded 2MB

###### 6. If the Type/Entity is invalid
