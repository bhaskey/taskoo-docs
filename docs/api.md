---
id: api
title: Web API Specification
sidebar_label: Web API Specification
---

# Task APIs

## Post Task

```json
POST request to api_endpoint/tasks
```

**Request Body**

<!--DOCUSAURUS_CODE_TABS-->
<!--main body-->

```JSON
{
  "title": "I want to get my daughters room painted",
  "details": "Please someone help me paint my dauhgter's room , it has to be painted in girlish colors.",
  "taskType": 1,
  "files": ["someBase64StringForAFile", "someAnotherBase64StringForAFile"],
  "mustHaves": ["string1", "string2", "string3"],
  "location": {},
  "dueDate": "01-10-2020",
  "dueTime": 2,
  "budget": {},
  "user": {},
  "category": "laundary services"
}
```
<!--location-->

```JSON
{
  "location":{
    "place_id" : "ChIJyWEHuEmuEmsRm9hTkapTCrk",
    "geometry":{
      "lng":"123.213",
      "lat":"23.3445345"
    },
    "name" : "Rhythmboat Cruises",
    "vicinity" : "Pyrmont Bay Wharf Darling Dr, Sydney"
  }
}
```

<!--user-->

```json
{
  "user":{
    "email":"user3@mail.com",
    "phone":"9000000003",
    "name":"user 3",
    "userId":1000,
    "imageUrl":"https://some-image-url-of-the-user"
  }
}
```

<!--budget-->

```json
{
  "budget":{
    "type":2,
    "amount":2000,
    "hours":0
  }
}
```

<!--END_DOCUSAURUS_CODE_TABS-->

> Note that task has `Location`, `User` & `Budget` Objects, please see their structures in tabs above.

> The location object is captured form [Google Places API](https://developers.google.com/places/web-service/search#find-place-responses)