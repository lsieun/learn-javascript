# jQuery Event Methods

URL: https://www.w3schools.com/jquery/jquery_ref_events.asp

Event methods **trigger** or **attach** a function to an event handler for the selected elements.

- `bind()`: Attaches event handlers to elements. **Deprecated in version 3.0**. Use the `on()` method instead.
- `click()`: Attaches/Triggers the click event
- `on()`: Attaches event handlers to elements
- `ready()`: Specifies a function to execute when the DOM is fully loaded

## `on()`

## `on` Example

Attach a `click` event to the `<p>` element:

```js
$("p").click(function(){
    console.log("click");
    $(this).hide();
});

$("p").on("click", function(){
  alert("The paragraph was clicked.");
});
```

## `ready()`

### `ready()` Syntax

Two syntaxes can be used:

```js
$(document).ready(function)
```

The `ready()` method can only be used on the current document, so no selector is required:

```js
$(function)
```

### `ready()` Example

Use `ready()` to make a function available after the document is loaded:

```js
$(document).ready(function(){
  $("button").click(function(){
    $("p").slideToggle();
  });
});
```


