# \<kbd\>

HTML `<kbd>` tag.

The HTML `<kbd>` tag, also known as the *keyboard input element*, is used to identify keystrokes that the user needs to make on a keyboard. Text incased in a `<kbd>` tag will be displayed in the browser's default *monospace* font.

## Syntax

An example of the HTML syntax is below:

```html
<kbd>Enter</kbd>
```

Result: <kbd>Enter</kbd>

## Attributes

This element supports *Global and Event Attributes in HTML.*

## Example 1

This example shows how the `<kbd>` tag operates as an inline element. Here it is incased inside the `<p>` tag and used to define text as *keyboard inputs.* Similar to how you would use the `<span>` element.

```html
<p>To reopen a closed Google tab press: <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>T</kbd></p>
```

Result:

<p>To reopen a closed Google tab press: <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>T</kbd></p>  
(This feature does not work in *incognito* mode.)

## Example 2

Here is another example that shows how to copy and paste highlighted text.

```html
<p>To copy highlighted text type: <kbd>Ctrl</kbd> + <kbd>C</kbd></p>
<p>To paste type: <kbd>Ctrl</kbd> + <kbd>V</kbd></p>
```

Result:

<p>To copy highlighted text type: <kbd>Ctrl</kbd> + <kbd>C</kbd></p>
<p>To paste type: <kbd>Ctrl</kbd> + <kbd>V</kbd></p>

## Browser Support

The `<kbd>` element is supported by all modern web browsers.

Google Chrome | Internet Explorer | Microsoft Edge | Firefox | Safari | Opera
--- | --- | --- | --- | --- | ---
Supported | Supported | Supported | Supported | Supported | Supported 

## Special Notes

Use it to identify individual key presses that should be pressed on a keypad. Keep in mind that the `<kbd>` element can be modified with CSS. Most browsers will display it with a default *monospace* font.