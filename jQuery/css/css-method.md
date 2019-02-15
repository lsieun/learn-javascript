# jQuery css() Method

URL: https://www.w3schools.com/jquery/jquery_css.asp

The `css()` method **sets** or **returns** one or more style properties for the selected elements.

## Return a CSS Property

To return the value of a specified CSS property, use the following syntax:

```js
css("propertyname");
```

The following example will return the background-color value of the FIRST matched element:

Example

```js
$("p").css("background-color");
```

## Set a CSS Property

To set a specified CSS property, use the following syntax:

```js
css("propertyname","value");
```

The following example will set the background-color value for ALL matched elements:

Example

```js
$("p").css("background-color", "yellow");
```

## Set Multiple CSS Properties

To set multiple CSS properties, use the following syntax:

```js
css({"propertyname":"value","propertyname":"value",...});
```

The following example will set a background-color and a font-size for ALL matched elements:

Example

```js
$("p").css({"background-color": "yellow", "font-size": "200%"});
```

## Example

让div隐藏和显示

```js
$('#div_id').css('display','none');
$('#div_id').css('display','block');
```

