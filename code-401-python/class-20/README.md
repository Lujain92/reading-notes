# Django CRUD and Forms
## Working with forms
An HTML Form is a group of one or more fields/widgets on a web page, which can be used to collect information from users for submission to a server. Forms are a flexible mechanism for collecting user input because there are suitable widgets for entering many different types of data, including text boxes, checkboxes, radio buttons, date pickers and so on. Forms are also a relatively secure way of sharing data with the server, as they allow us to send data in POST requests with cross-site request forgery protection.

### Form
The Form class is the heart of Django's form handling system. It specifies the fields in the form, their layout, display widgets, labels, initial values, valid values, and (once validated) the error messages associated with invalid fields. The class also provides methods for rendering itself in templates using predefined formats (tables, lists, etc.) or for getting the value of any element (enabling fine-grained manual rendering).

### Declaring a Form
The declaration syntax for a Form is very similar to that for declaring a Model, and shares the same field types (and some similar parameters).

Form data is stored in an application's forms.py file, inside the application directory. Create and open the file locallibrary/catalog/forms.py.


### Form Fields
Check out the following link for all the available form fields:

https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Forms#renew-book_form_using_a_form_and_function_view

### Validation
Django provides numerous places where you can validate your data. The easiest way to validate a single field is to override the method clean_() for the field you want to check. So for example, we can validate that entered renewal_date values are between now and 4 weeks by implementing clean_renewal_date() as shown below.

# References
1. https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Forms