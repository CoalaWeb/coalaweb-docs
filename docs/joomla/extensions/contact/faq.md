## List of Questions
1.  [How can I update the text starting: Do you have any idea in mind?](#q1)

***

#### <a class="doc-top" name="q1"></a>How can I update the text starting **Do you have any idea in mind?**

The complete text will look something like:

> Do you have any idea in mind? Contact us, we will give you the answer you expect. 

I have a feeling you got CoalaWeb Contact with your template and the text you are referring to is part of a template override found inside your template html directory.

This text isn't actually part of the original extension (I wouldn't hard code text into my extensions as it doesn't support multiple languages) but to remove or change it you will have to open up the following location and search for the text in question.

    templates/your-template-name/html/mod_coalawebcontact

***