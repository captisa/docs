# PowerApps Custom Connector



Captisa Forms allows you to build powerful online forms with workflows, conditional logic, duplicate detection rules, multi-level select, lookup, repeating panels, tabs, and accordions. Create views and filters and use them to analyze your data using charts or pivot grids, and then present them in the dashboard.

#### In this article

This connector is available in the following products and regions:

<table><thead><tr><th data-type="number">Service</th><th>Class</th><th>Regions</th></tr></thead><tbody><tr><td>null</td><td>Standard</td><td>All <a href="https://azure.microsoft.com/global-infrastructure/services/?products=logic-apps&#x26;regions=all">Logic Apps regions</a> except the following:<br>     -   Azure Government regions<br>     -   Azure China regions<br>     -   US Department of Defense (DoD)</td></tr><tr><td>null</td><td>Premium</td><td>All Power Automate regions except the following:<br>     -   US Government (GCC)<br>     -   US Government (GCC High)<br>     -   China Cloud operated by 21Vianet<br>     -   US Department of Defense (DoD)</td></tr><tr><td>null</td><td>Premium</td><td>All Power Apps regions except the following:<br>     -   US Government (GCC)<br>     -   US Government (GCC High)<br>     -   China Cloud operated by 21Vianet<br>     -   US Department of Defense (DoD)</td></tr></tbody></table>

| Contact |                                                                  |
| ------- | ---------------------------------------------------------------- |
| Name    | Captisa Form Support                                             |
| URL     | [https://captisa.com/contact-us](https://captisa.com/contact-us) |
| Email   | support@captisa.com                                              |

| Connector Metadata |                                                                                  |
| ------------------ | -------------------------------------------------------------------------------- |
| Publisher          | Connect Captisa                                                                  |
| Website            | [https://www.captisa.com](https://www.captisa.com)                               |
| Privacy policy     | [https://www.captisa.com/privacy-policy](https://www.captisa.com/privacy-policy) |
| Terms              | [https://www.captisa.com/terms](https://www.captisa.com/terms)                   |
| Categories         | Productivity;Sales and CRM                                                       |

### Prerequisites <a href="prerequisites" id="prerequisites"></a>

Create a free account on captisa.com.

### How to get credentials? <a href="how-to-get-credentials" id="how-to-get-credentials"></a>

1. Log in to your Captisa Forms account.
2. Navigate to System -> Settings.
3. Click on the 'Personal Access Token' button.
4. Click on the 'Generate Token' button.
5. Click the 'Copy' button to copy the token.

NOTE: Make sure to copy the personal access token. You won???t be able to see it again!

### Getting started with your connector <a href="getting-started-with-your-connector" id="getting-started-with-your-connector"></a>

Captisa Forms connector allows you to send form entries or updates to another app through triggers. A good example is when a new form entry is created in Captisa Forms, you can use a custom connector to create records in Dynamics 365, Marketo, etc. It also creates and updates actions that allow you to create or update records in your Captisa Forms account.

### Common errors and remedies <a href="common-errors-and-remedies" id="common-errors-and-remedies"></a>

### FAQ <a href="faq" id="faq"></a>

Q. Is Captisa Forms custom connector free to use?

A. Yes, our custom connector is free to use.

### Creating a connection <a href="creating-a-connection" id="creating-a-connection"></a>

The connector supports the following authentication types:

|                             |                                     |             |               |
| --------------------------- | ----------------------------------- | ----------- | ------------- |
| [Default](broken-reference) | Parameters for creating connection. | All regions | Not shareable |

#### Default

Applicable: All regions

Parameters for creating connection.

This is not a shareable connection. If the power app is shared with another user, another user will be prompted to create a new connection explicitly.

| Name    | Type         | Description              | Required |
| ------- | ------------ | ------------------------ | -------- |
| API Key | securestring | The API Key for this api | True     |

### Throttling Limits <a href="limits" id="limits"></a>

| Name                     | Calls | Renewal Period |
| ------------------------ | ----- | -------------- |
| API calls per connection | 100   | 60 seconds     |

### Actions <a href="actions" id="actions"></a>

| [Create an Entry](broken-reference) | Create an Entry |
| ----------------------------------- | --------------- |
| [Update an Entry](broken-reference) | Update an Entry |

#### Create an Entry <a href="create-an-entry" id="create-an-entry"></a>

Create an Entry.

**Parameters**

| Name        | Key    | Required | Type    | Description                             |
| ----------- | ------ | -------- | ------- | --------------------------------------- |
| Select form | formID | True     | string  | Select a form                           |
| body        | body   | True     | dynamic | This is the request body of the Webhook |

**Returns**

#### Update an Entry <a href="update-an-entry" id="update-an-entry"></a>

Update an Entry.

**Parameters**

| Name           | Key    | Required | Type    | Description                             |
| -------------- | ------ | -------- | ------- | --------------------------------------- |
| Select form    | formID | True     | string  | Select a form                           |
| Integration ID | id     | True     | string  | External data source primary ID         |
| body           | body   | True     | dynamic | This is the request body of the Webhook |

**Returns**

### Triggers <a href="triggers" id="triggers"></a>

| [When a form record is created](broken-reference) | This operation triggers a flow each time a form gets a new submission     |
| ------------------------------------------------- | ------------------------------------------------------------------------- |
| [When a form record is updated](broken-reference) | This operation triggers a flow each time an entry in your form is updated |

#### When a form record is created <a href="when-a-form-record-is-created" id="when-a-form-record-is-created"></a>

This operation triggers a flow each time a form gets a new submission.

**Parameters**

| Name        | Key    | Required | Type   | Description   |
| ----------- | ------ | -------- | ------ | ------------- |
| Select form | formID | True     | string | Select a form |

**Returns**

The outputs of this operation are dynamic.

#### When a form record is updated <a href="when-a-form-record-is-updated" id="when-a-form-record-is-updated"></a>

This operation triggers a flow each time an entry in your form is updated.

**Parameters**

| Name        | Key    | Required | Type   | Description   |
| ----------- | ------ | -------- | ------ | ------------- |
| Select form | formID | True     | string | Select a form |

**Returns**

The outputs of this operation are dynamic.

### Definitions <a href="definitions" id="definitions"></a>

#### Form Field Response <a href="formfieldresponse" id="formfieldresponse"></a>

| Name         | Path         | Type    | Description  |
| ------------ | ------------ | ------- | ------------ |
| content      | content      | object  | content      |
| duration     | duration     | string  | duration     |
| message      | message      | string  | message      |
| responseCode | responseCode | integer | responseCode |

### Feedback <a href="feedback" id="feedback"></a>

Submit and view feedback.&#x20;
