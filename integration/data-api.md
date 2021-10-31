# Data API

Captisa Forms Data API provides a development experience that can be used across a wide variety of programming languages, platforms, and devices. The purpose is to let you get your form entries and use whenever you see fit.

Captisa Forms API is a simple and powerful web service based on REST. It exposes your form entries via REST resources and HTTP GET method. For example, you can query set of fields from your form entries created today based on your View and Filter definitions. API supports JSON.

#### Getting Started

Below is an example to view form entries using PostMan

1\. Select a form from the form list.

2\. Select API button from the toolbar.

![API](https://captisacdn.blob.core.windows.net/img/api-1.PNG)

3\. Generate API token, then click Copy button. Paste token ID into your text editor.

![API](https://captisacdn.blob.core.windows.net/img/api-2.PNG)

4\. Select a View, then click Copy button. Paste view ID into your text editor

![API](https://captisacdn.blob.core.windows.net/img/api-3.PNG)

5\. Select a Filter, then click Copy button. Paste filter ID into your text editor

![API](https://captisacdn.blob.core.windows.net/img/api-4.PNG)

6\. Open PostMan

7\. Add a new tab and change request method to GET

8\. Paste ‘https://secure.captisa.com/api/data/v1/get’ in the URL field

9\. Select Header tab

10\. Add the following headers

**Key**: Token **Value**: \[Paste Token ID from Step 3]

**Key**: ViewId **Value**: \[Paste View ID from Step 4]

**Key**: FilterId **Value**: \[Paste Filter ID from Step 5]

**Key**: Content-Type **Value**: application/json

11\. Click Send button

![API](https://captisacdn.blob.core.windows.net/img/api-5.PNG)
