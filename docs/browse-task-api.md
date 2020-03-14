---
id: browse-task-api
title: Browse Task APIs
sidebar_label: Browse Task APIs
---

## Task List
Task in this API is lighter and doesn't have comments and offers. This is used for list views on Web and Mobile App.

```json
GET api_endpoint/tasks
```
**Response Body**

```json
[
  {
    "id":1,
    "title":"title of the task",
    "details":"some multiline description of the task",
    "taskStatus":"CREATED",
    "taskType":"OPEN",
    "mustHaves":["string1","string2","string3"],
    "dueDate":"01-10-2020",
    "dueTimeType":null,
    "budget":{},
    "category":"laundary services",
    "location":{},
    "user":{},
    "fileInfo":null,
    "noOfOffers":2
  },
  ...
]
```