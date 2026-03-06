---
title: Page Custom Validation Property
description: 
published: true
date: 2026-03-06T08:21:04.472Z
tags: 
editor: markdown
dateCreated: 2026-03-06T08:21:01.510Z
---

# Page Custom Validation

![rs-crud-addpage-pagecustomvalidation.webp](/assets/add-edit-properties/rs-crud-addpage-pagecustomvalidation.webp)

The **PageCustomValidation** property is a critical feature for developers who need to enforce complex business rules that go beyond standard field-level validation (like required fields or character limits). By providing a dedicated interface to write custom server-side logic, RadSystems Studio ensures that your application can handle unique data integrity requirements, such as checking for duplicate records across multiple tables or validating data against external business logic.

The **Dynamic Page Validation Statement** dialog provides a code editor to script your custom validation logic.

### Server-Side Execution

The custom validation code written in this window is executed on the server before any data is committed to the database. Consequently, the programming language and syntax you must use depend entirely on the **Backend Framework** (e.g., PHP Laravel or Node.js) selected during the initial project setup.

## Logic and Data Structure

The interface provides a clean function-based structure to handle your validation:

```
function validateAddPage(modeldata){
    // validation logic here
    // if (modeldata['field'] == 'invalid') { return 'Custom error message'; }
    return null;
}
```

**The modeldata Array**: All the fields and their user-submitted values are passed into the validation function as a `modeldata` array. This array contains data as key-value pairs, where the key is the field name and the value is the data entered by the user.

**Validation Logic**: Inside the function, you can write conditional statements to inspect the `modeldata` values.

- **Returning an Error**: If a validation rule is violated, the function must return the error message as a **string**. This string will then be displayed to the end-user on the form, preventing the submission.
    
- **Successful Validation**: If the data passes all your custom checks, the function is expected to return a **null** value. This signals to the server that it is safe to proceed with the record creation.
    