# Forms and JS Events

## HTML Forms

[HTML Forms](https://developer.mozilla.org/en-US/docs/Learn/Forms)

**Web forms** are one of the main points of interaction between a user and a website or application.

Forms are a very powerful tool for interacting with users — most commonly they are used for collecting data from users, or allowing them to control a user interface.

**action** - attribute defines the location (URL) where the form's collected data should be sent when it is submitted.

**method** - attribute defines which HTTP method to send the data with (usually get or post).

### Designing a Form

The bigger your form, the more you risk frustrating people and losing users. Keep it simple and stay focused: ask only for the data you absolutely need.

### Form Elements

- **form** - defines a form. It's a container element like a section or footer element, but specifically for containing forms.
- **label** - For usability and accessibility, we include an explicit label for each form control. **for** attribute on all these elements which takes the **id** of the form control with which it is associated.
- **input** - uses type attribute. Extremely important because it defines the way the input element appears and behaves.
- **textarea** - input field for the message.

## Button

 Allow the user to send, or "submit", their data once they have filled out the form.

## JS EventListeners

[Introduction to Events](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Events)

Events are things that happen in the system you are programming — the system produces (or "fires") a signal of some kind when an event occurs, and provides a mechanism by which an action can be automatically taken (that is, some code running) when the event occurs.

### addEventListener

Objects that can fire events have an addEventListener() method. 

Will need to have the event handler and the event listener arguments???

### Event Object

Sometimes, inside an event handler function, you'll see a parameter specified with a name such as event, evt, or e.

**Event Object** - automatically passed to event handlers to provide extra features and information. **target** property of the event object is always a reference to the element the event occured upon.