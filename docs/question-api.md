---
id: question-api
title: Question APIs
sidebar_label: Question APIs
---

## Ask a Question
> A question can have replies to it. The replies to a question can tracked by `parentId`. More details on [Task Details](task-details-api.md)

```json
POST api_endpoint/questions
```
> Please see the `user` object on [task api](api.md)
**Request Body**
```json
{
  "user":{},
  "taskId":1,
  "questionText":"question text goes here this is the question about the task bla bla",
  "parentId":1
}
```