---
title: "Adding Headers to a PDF Document"
type: docs
url: /adding-headers-to-a-pdf-document/
weight: 10
---

# **Introduction**
Aspose.PDF Cloud allows you to add Header to a PDF Document. Aspose.PDF Cloud supports adding Text and Image Header to a PDF Document
### **API Information**

|**API**|**Type**|**Description**|**Swagger Link**|**Request DTO**|
| :- | :- | :- | :- | :- |
|/pdf/{name}/header/text|POST|Add document Text Header|[PostDocumentTextHeader](https://apireference.aspose.cloud/pdf/#!/HeaderFooter/PostDocumentTextHeader)|[TextHeader](https://github.com/aspose-pdf-cloud/aspose-pdf-cloud-php/blob/master/docs/TextHeader.md)|
|/pdf/{name}/header/image|POST|Add document Image Header|[PostDocumentImageHeader](https://apireference.aspose.cloud/pdf/#!/HeaderFooter/PostDocumentImageHeader)|[ImageHeader](https://github.com/aspose-pdf-cloud/aspose-pdf-cloud-php/blob/master/docs/ImageHeader.md)|
### **cURL Example**
**Example for adding a Text Header to a PDF Document**

{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}

{{< tab tabNum="1" >}}

**Get Authentication Token**

```java

curl -v "https://api.aspose.cloud/connect/token" \
-X POST \
-d "grant_type=client_credentials&client_id=xxxx&client_secret=xxxx" \
-H "Content-Type: application/x-www-form-urlencoded" \
-H "Accept: application/json"

```

```java

curl -v "http://api.aspose.cloud/v3.0/pdf/4pages.pdf/header/text" -X POST -H "Content-Type: application/json" -H "Accept: application/json" -H "Authorization: Bearer XgPIwP9GyHhPw4bE4naCtOv6XXZSrtgHJWuXIXDJTwd6HAk7KipxTNOicRzzXu5JUpCbli9OAdmQEssSEm4Hx8wZhHsCop9mj3S4no9cx3pa9FbJTjC64CPann7APzfb4ajqcJXrOVu4Lou1OQwaI2TItRnmNGDQF7Mucj8RWSc8zsbEEzbRw22i8lbqu_40_a7CJugilsxs7OGkXel5wqKzXDJbIbMUPHEHQWQJPyfkh9HdKqnkdl0LkyzMQFs5swkzjmekDqACZJNpAqxQDtqVy7248hFlRPL6KfIRYypic8gRdig716KKuSFRiMyt3xgA5_cNcgH4EAXlZSCpKssy08nEC1EomaD4pmp65zLP6ISbBm4lp2pJjqO9aJiamQuQEa1XlSkyGLg2LluNVX5TyRq_Mn8sKIAjBf7eI02Ebzbt"  --ssl-no-revoke -d "{'Background': true, 'HorizontalAlignment': 'Center', 'Opacity': 1, 'Rotate': 'None', 'RotateAngle': 10, 'XIndent': 0, 'YIndent': 0, 'Zoom': 1, 'TextAlignment': 'Center', 'Value': 'Header', 'TextState': {'FontSize': 14, 'Font': 'Arial Bold', 'ForegroundColor': {'A': 0, 'R': 0, 'G': 255, 'B': 0 }, 'BackgroundColor': {'A': 0, 'R': 255, 'G': 0, 'B': 0 }, 'FontStyle': 'Bold'}, 'LeftMargin': 1, 'TopMargin': 20, 'RightMargin': 2 }"

```

{{< /tab >}}

{{< tab tabNum="2" >}}

```java
{
  "Code": 201,
  "Status": "Created"
}
```

{{< /tab >}}

{{< /tabs >}}

**Example for adding a Image Header to a PDF Document**

{{< tabs tabTotal="2" tabID="5" tabName1="Request" tabName2="Response" >}}

{{< tab tabNum="1" >}}

**Get Authentication Token**

```java

curl -v "https://api.aspose.cloud/connect/token" \
-X POST \
-d "grant_type=client_credentials&client_id=xxxx&client_secret=xxxx" \
-H "Content-Type: application/x-www-form-urlencoded" \
-H "Accept: application/json"

```

```java

curl -v "http://api.aspose.cloud/v3.0/pdf/4pages.pdf/header/text" -X POST -H "Content-Type: application/json" -H "Accept: application/json" -H "Authorization: Bearer XgPIwP9GyHhPw4bE4naCtOv6XXZSrtgHJWuXIXDJTwd6HAk7KipxTNOicRzzXu5JUpCbli9OAdmQEssSEm4Hx8wZhHsCop9mj3S4no9cx3pa9FbJTjC64CPann7APzfb4ajqcJXrOVu4Lou1OQwaI2TItRnmNGDQF7Mucj8RWSc8zsbEEzbRw22i8lbqu_40_a7CJugilsxs7OGkXel5wqKzXDJbIbMUPHEHQWQJPyfkh9HdKqnkdl0LkyzMQFs5swkzjmekDqACZJNpAqxQDtqVy7248hFlRPL6KfIRYypic8gRdig716KKuSFRiMyt3xgA5_cNcgH4EAXlZSCpKssy08nEC1EomaD4pmp65zLP6ISbBm4lp2pJjqO9aJiamQuQEa1XlSkyGLg2LluNVX5TyRq_Mn8sKIAjBf7eI02Ebzbt"  --ssl-no-revoke -d "{'Background': true, 'HorizontalAlignment': 'Center', 'Opacity': 1, 'Rotate': 'None', 'RotateAngle': 10, 'XIndent': 0, 'YIndent': 0, 'Zoom': 1, 'TextAlignment': 'Center', 'filename': 'Koala.jpg', 'TextState': {'FontSize': 14, 'Font': 'Arial Bold', 'ForegroundColor': {'A': 0, 'R': 0, 'G': 255, 'B': 0 }, 'BackgroundColor': {'A': 0, 'R': 255, 'G': 0, 'B': 0 }, 'FontStyle': 'Bold'}, 'LeftMargin': 1, 'TopMargin': 20, 'RightMargin': 2 }"

```

{{< /tab >}}

{{< tab tabNum="2" >}}

```java
{
  "Code": 201,
  "Status": "Created"
}
```

{{< /tab >}}

{{< /tabs >}}
