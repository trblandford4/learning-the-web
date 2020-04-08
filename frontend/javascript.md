# Contents

1. [DOM Manipulation](#Dom-Manipulation)

# Dom Manipulation

## The Document Object Model

- What happens when you request a website?

  1. HTML is received
  2. HTML tags are converted to tokens
  3. tokens are converted to Nodes
  4. Nodes are converted to the DOM

- The DOM is a model (representation) of the relationships and attributes of the HTML markup

  > Document Object Model => Object Model of the Document

- The `document` object is provided by the browser

  - not part of JavaScript
  - already exists and freely accessible to JS code

- W3C standard specifications

  - Core Specification
  - Events Specification
  - Style Specification
  - Validation Specification
  - Load and Save Specification
  - [All specs defined by W3C here](https://www.w3.org/standards/techs/dom#w3c_all)

- HTML Nodes and Elements have all their properties and methods defined by the [Web API Interfaces](https://developer.mozilla.org/en-US/docs/Web/API)

## Browser Events

- EventTarget

  > an interface implemented by objects that can receive events and may have listeners for them.

- Event Listeners

  - Need 3 things:
    1. An event **target**
    2. the **type** of event to listen for
    3. function to run when the event occurs: **listener**

- Event Phases

  - **Capturing**: can configure listener to run during this phase before reaching target
  - **At target**: when EventTarget is reached, switches to Bubbling phase
  - **Bubbling**: runs listener after target is reached, then "bubbles" back up to the parent until it reaches the document [*default*]

- DOMContentLoaded: The DOM is built incrementally and some elements may not be "ready" when you try to manipulate them.

## Performance

- Adding Page Content
- Reflow & Repaint
- The Call Stack
- The Event Loop
- setTimeout

## Resources

- [Udacity: Javascript and the DOM](https://www.udacity.com/course/javascript-and-the-dom--ud117)