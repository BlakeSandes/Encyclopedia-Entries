#window.pageYOffset

The `window.pageYOffset` returns the number in pixels that the document has already scrolled vertically in relation to the top of the document window.



The   `pageYOffset` property is useful when used with any of the builtin realitive window functions such as window.scrollBy, window.scrollByLines, or window.scrollByPages. The property can be used to check if the document is being scrolled in the `y` axis and the relative window functions can be acted upon when the conditions are met. 

The `pageYOffset` property is an alias for the `scrollY` property.

For example: 

```
window.pageYOffset == window.scrollY; //-> Returns true
```

Use `pageYOffset` instead of `scrollY` for cross-browser compatibility, though Internet Explorer 9 and later do not support either property.



## Syntax

```
var y = window.pageYOffset 
```

console.log(y) 
> Outputs the number of pixels 
