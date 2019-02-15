# jQuery ready() Method

URL: https://www.w3schools.com/jquery/event_ready.asp

## Example

Use `ready()` to make a function available after the document is loaded:

```js
$(document).ready(function(){
  $("button").click(function(){
    $("p").slideToggle();
  });
});
```

## Definition and Usage

The ready event occurs when the DOM (document object model) has been loaded.

Because this event occurs after the document is ready, it is a good place to have all other jQuery events and functions. Like in the example above.

The `ready()` method specifies what happens when a ready event occurs.

**Tip**: The `ready()` method should not be used together with `<body onload="">`.

## Syntax

Two syntaxes can be used: 

```js
$(document).ready(function)
```

The `ready()` method can only be used on the current document, so no selector is required:

```js
$(function)
```

## The Document Ready Event

```js
$(document).ready(function(){

  // jQuery methods go here...

});
```

This is to prevent any jQuery code from running before the document is finished loading (is ready).

It is good practice to wait for the document to be fully loaded and ready before working with it. This also allows you to have your JavaScript code before the body of your document, in the `<head>` section.

Here are some examples of actions that can fail if methods are run before the document is fully loaded:

- Trying to hide an element that is not created yet
- Trying to get the size of an image that is not loaded yet

Tip: The jQuery team has also created **an even shorter method** for the **document ready event**:

```js
$(function(){

  // jQuery methods go here...

});
```

Use the syntax you prefer. We think that the document ready event is easier to understand when reading the code.
