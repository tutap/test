# Create class - POST

POST /v2/class

## Description



* [Request Payloads](#request-payloads)
* [Response Payloads](#response-payloads)

|                                       |                                                 |
| ------------------------------------- | ----------------------------------------------- |
| HTTP Method                           | Post                                         |
| API                                   | Class                                           |
| Api Version                           | 2.0.0.3                                         |
| Resource Version                      | 1                                               |
| Summary                               |                                       |
| Base Path                             | /v2/class                                     |
| Resource                              | Create class                                      |
| Endpoint URL                          | https://api-dev.test.com/v2/class              |
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
| Classes |  |  -  | No | No | No | No |  -  | Data Type : object<br>  |
| >Class name |  | T | **YES** | No | No | No |  -  | Data Type : string<br> Min. length :  - <br> Max. length : No<br> Regex :  - <br>  |



#### Json sample
```
{
  "className": "T"
}
```


#### Json Schema
```
{
  "$schema": "http://json-schema.org/draft-04/schema#",
  "title": "Classes",
  "type": "object",
  "properties": {
    "className": {
      "title": "Class name",
      "type": "string",
      "items": []
    }
  },
  "required": [
    "className"
  ],
  "items": []
}
```

---