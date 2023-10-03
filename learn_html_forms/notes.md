
<!-- WHY learn html forms?  -->
You can use HTML forms to collect information from people who visit your webpage.

<!-- what viewport height? -->
The vh unit stands for viewport height, and is relative to 1% of the height of the viewport.

<!-- 0 Margin to hide scrolls -->
Q. How to get rid of horizontal scroll-bar?
setting the body default margin added by some browsers to 0.

<!-- Method attr  -->
The method attribute specifies how to send form-data to the URL specified in the action attribute.

<!-- Changing display of element  -->
The rem unit stands for root em, and is relative to the font size of the html element.

As label elements are inline by default, they are all displayed side by side on the same line, making their text hard to read. To make them appear on separate lines, add display: block to the label element, and add a margin of 0.5rem 0, to separate them from each other.

<!-- Best accessibility practices -->
Following accessibility best practices, link the input elements and the label elements together using the for attribute.

This association is essential for accessibility because it helps screen readers and other assistive technologies provide meaningful information to users.

<!-- Types of input -->
Specifying the type attribute of a form element is important for the browser to know what kind of data it should expect. If the type is not specified, the browser will default to text.

Give the first two input elements a type attribute of text, the third a type attribute of email, and the fourth a type attribute of password.

The email type only allows emails with a @ and a . in the domain. The password type obscures the input, and warns if the site does not use HTTPS.

<!-- Submit input -->
The first input element with a type of submit is automatically set to submit its nearest parent form element.

To handle the form submission, after the last fieldset element add an input element with the type attribute set to submit and the value attribute set to Submit.

<!--  Custom Validation -->
Certain type attribute values come with built-in form validation. For example, type="email" requires that the value be a valid email address.

Add custom validation to the password input element, by adding a minlength attribute with a value of 8. Doing so prevents inputs of less than 8 characters being submitted.

<!-- Regex for password type -->
With type="password" you can use the pattern attribute to define a regular expression that the password must match to be considered valid.

<!-- Option to select one choice -->
Users will be allowed to choose either a Personal Account or Business Account.

To do this, within each of the first two label elements, add one input element with type="radio".

You only want one radio input to be selectable at a time. However, the form does not know the radio inputs are related.

To relate the radio inputs, give them the same name attribute with a value of account-type. Now, it is not possible to select both radio inputs at the same time.

<!-- Option to choose multiple choices -->
For the terms and conditions, add an input with a type of checkbox to the third label element.
Make this input element required because users should not sign up without reading the terms and conditions.

<!-- Why need value attr -->
Submitting the form with an option selected would not send a useful value to the server. As such, each option needs to be given a value attribute. Without which, the text content of the option will be submitted to the server.

<!-- how to pass multiline text: textarea element -->
The textarea element acts like an input element of type text, but comes with the added benefit of being able to receive multi-line text, and an initial number of text rows and columns.

Users will be able to register with a bio.
Add a label with the text Provide a bio: at the end of the fieldset. Add a textarea element inside the label element. Note that the textarea requires a closing tag.

<!-- why give name attr -->
With form submissions, it is useful, and good practice, to provide each submittable element with a name attribute. This attribute is used to identify the element in the form submission.

<!-- select last element of a specific type -->
using the last-of-type CSS pseudo-class, like this:
    p:last-of-type { }

<!-- attribute selector -->
input[name="givenName"]{}