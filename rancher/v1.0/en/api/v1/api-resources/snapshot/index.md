---
title: API
layout: rancher-api-v1-default-v1.0
version: v1.0
lang: en
apiVersion: v1
---

## snapshot



### Resource Fields

#### Writeable Fields

Field | Type | Create | Update | Default | Notes
---|---|---|---|---|---
description | string | Optional | Yes | - | 
name | string | Optional | Yes | - | 
volumeId | [volume]({{site.baseurl}}/rancher/{{page.version}}/{{page.lang}}/api/{{page.apiVersion}}/api-resources/volume/) | Yes | - | - | 


#### Read Only Fields

Field | Type   | Notes
---|---|---
accountId | [account]({{site.baseurl}}/rancher/{{page.version}}/{{page.lang}}/api/{{page.apiVersion}}/api-resources/account/)  | The unique identifier for the associated account
created | date  | The date of when the snapshot was created.
id | int  | The unique identifier for the snapshot
kind | string  | 
managedVolumeUUID | string  | 
removed | date  | The date of when the snapshot was removed
state | enum  | The current state of the snapshot. The options are `backed-up`, `backing-up`, `created`, `creating`, `removed`, `removing`, `requested`.
transitioning | enum  | Whether or not the snapshot is in a transitioning state
transitioningMessage | string  | The message to show while in a transitioning state
transitioningProgress | int  | The percentage remaining in the transitioning process of the snapshot
uuid | string  | The universally unique identifier for the snapshot. This will always be unique across Rancher installations.


<br>
