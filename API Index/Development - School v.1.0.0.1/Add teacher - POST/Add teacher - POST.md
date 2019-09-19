# Add teacher - POST

POST /v1/school

## Description



* [Request Payloads](#request-payloads)
* [Response Payloads](#response-payloads)

|                                       |                                                 |
| ------------------------------------- | ----------------------------------------------- |
| HTTP Method                           | Post                                         |
| API                                   | School                                           |
| Api Version                           | 1.0.0.1                                         |
| Resource Version                      | 1                                               |
| Summary                               |                                       |
| Base Path                             | /v1/school                                     |
| Resource                              | Add teacher                                      |
| Endpoint URL                          | https://api-dev.test.com/v1/school              |
| Service Status                        | Unknown                                         |
| Legislative / Regulatory / Compliance |                                             |
| Firewalls Details                     |                                              |
| Security Certificate Details          |                                              |
| Vendor or Partner Considerations      |                                             |

## Request Payloads

### Request Header


N/A
---

### Query Params


N/A
---

### Request Body

#### Payload 



| Parameter | Description | Sample | PII | Sensitive | Unique Identifier | Mandatory | Default | Details |
| :----- | :-----: | :-----: | :-----: | :-----: | :-----: | :-----: | :-----: | :----- |
| Teacher |  |  -  | No | No | No | No |  -  | Data Type : object<br>  |
| >Person | A person |  -  | No | No | No | No |  -  | Data Type : object<br>  |
| >>Person Id | This is the id of person | 46b1cbfb-5b57-40eb-9615-9902f49c2d0e | **YES** | **YES** | **YES** | No |  -  | Data Type : string<br> Min. length :  - <br> Max. length : No<br> Regex :  - <br>  |
| >>First Name |  | David | **YES** | **YES** | No | No |  -  | Data Type : string<br> Min. length : 1<br> Max. length : No<br> Regex :  - <br>  |
| >>Middle Name |  |  -  | No | No | No | No |  -  | Data Type : string<br> Min. length :  - <br> Max. length : No<br> Regex :  - <br>  |
| >>Last Name |  | Yonan | **YES** | **YES** | No | No |  -  | Data Type : string<br> Min. length : 1<br> Max. length : No<br> Regex :  - <br>  |
| >>DoB |  | 1/1/1999 | No | **YES** | No | No |  -  | Data Type : string<br> Min. length :  - <br> Max. length : No<br> Regex :  - <br>  |



#### Json sample
```
{
  "person": {
    "personId": "46b1cbfb-5b57-40eb-9615-9902f49c2d0e",
    "firstName": "David",
    "middleName": null,
    "lastName": "Yonan",
    "dob": "1/1/1999"
  }
}
```


#### Json Schema
```
{
  "$schema": "http://json-schema.org/draft-04/schema#",
  "title": "Teacher",
  "type": "object",
  "properties": {
    "person": {
      "title": "Person",
      "description": "<p>A person</p>",
      "type": "object",
      "properties": {
        "personId": {
          "title": "Person Id",
          "description": "<p>This is the id of person</p>",
          "type": "string",
          "items": []
        },
        "firstName": {
          "title": "First Name",
          "type": "string",
          "items": [],
          "minLength": 1
        },
        "middleName": {
          "title": "Middle Name",
          "type": "string",
          "items": []
        },
        "lastName": {
          "title": "Last Name",
          "type": "string",
          "items": [],
          "minLength": 1
        },
        "dob": {
          "title": "DoB",
          "type": "string",
          "items": []
        }
      },
      "required": [
        "personId",
        "firstName",
        "lastName",
        "dob"
      ],
      "items": []
    }
  },
  "items": []
}
```

---