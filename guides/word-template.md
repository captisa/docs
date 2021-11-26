# Word Template

After creating and importing Office Word templates into Captisa Forms, users can automatically, with one click, generate standardized documents populated with data or send them as attachments to emails. This feature has some special considerations you should know about to create Word templates successfully.&#x20;

#### Step 1: Create a Word Template

1\. Go to form entries.

2\. Click on Word Template > Download Template.

![](https://captisa.com/wp-content/uploads/2020/02/DownloadTemplate.png)

&#x20;

#### Step 2: Enable the Developer Tab

1\. Open the Word template file. At this point, the document appears to be blank.

![](https://captisa.com/wp-content/uploads/2020/02/EnableDeveloperTab.png)

2\. Go to File > Options > Customize Ribbon, and then enable Developer.

![](https://captisa.com/wp-content/uploads/2020/02/EnableDeveloperTab2.png)

3\. Click OK.

The developer now appears in the Word ribbon.

&#x20;

#### Step 3: Define the Word template

1\. In your Word template, click Developer > XML Mapping Pane.

![](https://captisa.com/wp-content/uploads/2020/02/XmlMappingPane.png)

The default XML Schema is selected.

![](https://captisa.com/wp-content/uploads/2020/02/DefaultSchema.png)

2\. Select Captisa Forms XML schema – “urn:captisa-forms/document-template/forms/1/”

![](https://captisa.com/wp-content/uploads/2020/02/CaptisaFormXmlSchema.png)

3\. Expand Document Template, right-click the form field, and then click Insert Content Control > Plain Text.

![](https://captisa.com/wp-content/uploads/2020/02/InsertContentControl.png)

4\. The form field is added to the Word template.

![](https://captisa.com/wp-content/uploads/2020/02/FormFieldAdded-e1581193087557.png)

&#x20;

A completed template might look like this:

![](https://captisa.com/wp-content/uploads/2020/02/CompletedTemplate.png)

&#x20;

Your form might have a repeating section. For example, a student can have more than one emergency contact. To include all the data in your Word template, set the content control field to repeat.

&#x20;

**Set form fields to repeat**

1\. Put the form fields with repeating data in a table row.

2\. Select the entire table row in the table.

![](https://captisa.com/wp-content/uploads/2020/02/RepeatingSection.png)

3\. In the XML Mapping Pane, right-click the repeating section field, select Insert Content Control, and then click Repeating.

![](https://captisa.com/wp-content/uploads/2020/02/RepeatingSection2.png)

&#x20;

#### Step 4: Upload the Word template back

When you have your Word template built the way you want, save it so you can upload it into Captisa Forms Cloud.

&#x20;

1\. Go to form entries.

2\. Click on Word Template > Upload Template.

3\. Select your Word template.

4\. Click Open.

&#x20;

You are now ready to view or download a document.

1\. Go to form entries.

2\. Select the Word Template.

3\. Click Word or PDF to download the document or View it.

![](https://captisa.com/wp-content/uploads/2020/02/DownloadDocument.png)

&#x20;

An example of PDF document

![](https://captisa.com/wp-content/uploads/2020/02/GeneratedWordDocument.png)

&#x20; &#x20;

### Attach generated PDF document to the email

It is easy to attach generated PDF documents to the email.

&#x20;

1\. Create a Workflow with an action of Send Email.

2\. In the Attachments field, select one (1) or more Word templates.

A Workflow with generated PDF document attachment might look like this:

![](https://captisa.com/wp-content/uploads/2020/02/AttachWordDocumentToEmail.png)
