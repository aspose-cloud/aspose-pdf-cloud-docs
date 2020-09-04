---
title: "Adding a RadioBox Control to a PDF Document"
type: docs
url: /adding-a-radiobox-control-to-a-pdf-document/
weight: 10
---

# **Introduction**
Aspose.PDF Cloud allows you to add a RadioBox fields to a PDF Document. The Aspose.PDF Cloud API provides the following methods
### **API Information**

|**API**|**Type**|**Description**|**Swagger Link**|
| :- | :- | :- | :- |
|/pdf/{name}/fields/radiobutton|POST|Post Document Radiio Button fields|[PostRadioButtonFields](https://apireference.aspose.cloud/pdf/#/Fields/PostRadioButtonFields)|
### **cURL Example**
{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}

{{< tab tabNum="1" >}}

**Get Authentication Token**

```java

curl -v "https://api.aspose.cloud/connect/token" \

-X POST \

-d "grant\_type=client\_credentials&client\_id=xxxx&client\_secret=xxxx" \

-H "Content-Type: application/x-www-form-urlencoded" \

-H "Accept: application/json"

```

```java

curl -X POST "https://api.aspose.cloud/v3.0/pdf/4pages.pdf/fields/radiobutton" \

-H "accept: application/json" \

-H "authorization: Bearer <jwt token>" \

-H "Content-Type: application/json" \

-d "[ { \"PartialName\": \"test1Field1\", \"Rect\": { \"LLX\": 100, \"LLY\": 100, \"URX\": 160, \"URY\": 140 }, \"PageIndex\": 1, \"IsGroup\": false, \"Color\": { \"A\": 255, \"R\": 255, \"G\": 0, \"B\": 0 }, \"Margin\": { \"Left\": 0, \"Right\": 0, \"Top\": 0, \"Bottom\": 0 }, \"Highlighting\": \"None\", \"HorizontalAlignment\": \"None\", \"VerticalAlignment\": \"None\", \"RadioButtonOptionsField\": [ { \"Rect\": { \"LLX\": 100, \"LLY\": 130, \"URX\": 160, \"URY\": 140 }, \"PageIndex\": 1, \"IsGroup\": false, \"Highlighting\": \"None\", \"HorizontalAlignment\": \"None\", \"VerticalAlignment\": \"None\", \"OptionName\": \"1\", \"Style\": \"Square\" }, { \"Rect\": { \"LLX\": 150, \"LLY\": 120, \"URX\": 160, \"URY\": 130 }, \"PageIndex\": 1, \"IsGroup\": false, \"Highlighting\": \"None\", \"HorizontalAlignment\": \"None\", \"VerticalAlignment\": \"None\", \"OptionName\": \"2\", \"Style\": \"Circle\" } ], \"Style\": \"Cross\", \"Selected\": 1 }]"

```

{{< /tab >}}

{{< tab tabNum="2" >}}

```java

{

   "Code":200,

   "Status":"OK"

}

```

{{< /tab >}}

{{< /tabs >}}
# **SDK Source**
The Aspose.PDF Cloud SDKs can be downloaded from the following page: [Available SDKs](/available-sdks-html/)
