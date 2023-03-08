# Forms and JS Events

This topic is important to me because I want to get better at being able to let users be able to put things into my webpage.

## References

<https://developer.mozilla.org/en-US/docs/Learn/Forms/Your_first_form>.
<https://developer.mozilla.org/en-US/docs/Learn/Forms/How_to_structure_a_web_form>.
<https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Events>.
<https://developer.mozilla.org/en-US/docs/Learn/Forms/HTML5_input_types>.
<https://developer.mozilla.org/en-US/docs/Web/Events>.

## Web Forms

**Web forms** are the main points of interaction between a user and a website/application.

Forms let users enter data.
Its sent to a web server for processing and storage.

Or used to update the interface client side.

A web form's HTML is made up of one or more form controls.
(Sometimes called widgets).
HTML Forms!

**Coding Advice for Forms** - Step back and think about your form, keep it simple and only ask for data you absolutely need.

All forms start with the form element <>.

This defines a form, it contains the forms and also supports specific attributes. Standard practice is to add action and method.

**Action Attribute** - defines the location where the forms collected data should be submitted.

**Method Attribute** - defines which http method to send the data with (get or post usally).

Theres 3 elements that a form usually uses : label, input, and textarea.

**Input** is used for the name, a single line text field.
Its also used for the email and message box.
The input field for a message is an **textarea** a multiline text field.

    <form action="/my-handling-form-page" method="post">
    <ul>
    <li>
      <label for="name">Name:</label>
      <input type="text" id="name" name="user_name" />
    </li>
    <li>
      <label for="mail">Email:</label>
      <input type="email" id="mail" name="user_email" />
    </li>
    <li>
      <label for="msg">Message:</label>
      <textarea id="msg" name="user_message"></textarea>
    </li>
    </ul>
    </form>

We use li elements to structure the code and make styling easier, for accessibility we include an explicit label for each form control.

The label has a for attribute, which links to the id of the input, this is how you associate a form control with its label.

On the input element the attribute **type** is the most important, it defines the way the input element appears and behaves.

The **Button** element accepts a type attri- submit, reset, or button.

Submit sends the data to the web page defined by the action attri of the form element.

A click on a reset resets all form widges. (Bad Practice).

Button type does nothing! This allows you to give it custom jobs in JS.

**Name** attribute is used on each form widget to title the data being sent through.

## Structuring Forms

The **form** element defines a form and attributes that determine the form's behavior.

**Fieldset** element is a convenient way to create groups of widgets that share the same purpose. (styling and semantic).

Labeling a fieldset means including a legend element below the opening of the fieldset tag.

The **legend** text content will describe the purpose of the fieldset.

**Radio** buttons should always be nested inside a fieldset element.

The **label** element is the formal way to define a form.

Its the most important for accessible forms.

### Form Questions

1.  It lets use use data and manage user interaction.
2. Accessibility and the right attributes.
3. Fieldset(good for widgets that share the same purpose), Label (the formal way to define a form), button (allows actions to be performed), input (defines how the form behaves), textarea (for the information in the forms inputs)

## JavaScript Events

Events are things that happen in the system you are programming, it sends a signal.

To react to an event, you attach an event handler.

An **event handler** is a block of code, that runs when the event fires.

When that block of code is defined to run in response to an event, we say we are registering an event handler.

Event handlers = event listeners.

The listener listens out for the event happening, and the handler is the code run in response.

    const btn = document.querySelector("button");

    function random(number) {
    return Math.floor(Math.random() * (number + 1));
    }

    btn.addEventListener("click", () => {
    const rndCol = `rgb(${random(255)}, ${random(255)}, ${random(255)})`;
    document.body.style.backgroundColor = rndCol;
    });

If button is clicked, do this!

**addEventListener()** method listens for the event fire.

the click event can be changed to different things such as focus, blur, dblclick, mouseover, and mouseout.

**removeEventListener()** lets you remove the event you applied before.

    btn.removeEventListener("click", changeBackground);

its removed!

Other way event handlers can be removed is by passing an AbortSignal to addEventListener().

and then later calling abort() on the controller owning the AbortSignal.

    const controller = new AbortController();

    btn.addEventListener(
    "click",
    () => {
    const rndCol = `rgb(${random(255)}, ${random(255)}, ${random(255)})`;
    document.body.style.backgroundColor = rndCol;
    },
    { signal: controller.signal }
    ); // pass an AbortSignal to this handler

    and then

    controller.abort(); // removes any/all event handlers associated with this controller

You can also add multiple isteners for a single event.

**Event Object** Helps pass event handlers to provide extra features and info automatically.

    const btn = document.querySelector("button");

    function random(number) {
      return Math.floor(Math.random() * (number + 1));
    }

    function bgChange(e) {
    const rndCol = `rgb(${random(255)}, ${random(255)}, ${random(255)})`;
    e.target.style.backgroundColor = rndCol;
    console.log(e);
    }

    btn.addEventListener("click", bgChange);

preventDefault() is used in an event listener to prevent its normal actions and let your stuff go.

It can be used for form validation and many other ways.

Event bubbling is a phenomenon that occurs when an event is triggered on a nested element within a parent element that also has an event listener. The event first triggers on the nested element and then "bubbles up" through its parent elements in the DOM tree, triggering any event listeners attached to those parent elements.

Event bubbling can be useful for handling events on multiple elements with a single event listener.

### Event Questions

1. Events are like when you press an elevator button, once the button is clicked an action is completed.
2. addEventListener(type, listener)
3. It helps execute code more quickly and everything is more organized.
4. Event capturing is the reverse of event bubbling. Event bubbling starts from where the event is called and goes up the DOM tree, and reverse for event capturing.

## Things I want to know more about

How to use event listeners for objects

I want to know more about the complexity of listeners.

