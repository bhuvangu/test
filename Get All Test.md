#Get All Test

Description
---
Returns the list of all *Live* tests.

URL
---

```
Method Type: GET
https://BASE-URL/harvest/api/v1/getLiveTests/{pageNo}
```

Sample Response Data
---
Returns a array of Object, where each object represent a test live.
```
[
    {
        "testId": 343,  // Test Id
        "testName": "public2", // Test name
        "testOpenTime": 1520317324138, // When did the test opened timestamp in GMT
        "testCloseTime": 1521526860000,// When will the test close timestamp in GMT
        "totalMarks": 8,  // total marks for the test
        "cutOffMarks": 0,  // cut off Marks for the test
        "candidateReportNotificationUrl": null  //  whenever candidate completes the test thisWebhook will be called to notify.
    },
    {
        "testId": 318,
        "testName": "hello127",
        "testOpenTime": 1519985460232,
        "testCloseTime": 1521367800000,
        "totalMarks": 4,
        "cutOffMarks": 0,
        "candidateReportNotificationUrl": null
    },
    {
        "testId": 315,
        "testName": "hello126",
        "testOpenTime": 1519985444680,
        "testCloseTime": 1520763000000,
        "totalMarks": 4,
        "cutOffMarks": 0,
        "candidateReportNotificationUrl": null
    }
]
```

Possible Exceptions
---
```
Status Code: 602
{"errorMessage": "Page number can't be negative"}
```

```
Status Code: 600
{"errorMessage": "Page number can't be negative"}
or 
{"errorMessage": "apikey not mapped to a user"}
```



```

