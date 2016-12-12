# window.location

A read-only object that returns a `location`property.

If you need to get information about a `window`'s URL (`location`) or redirect the browser to a new page, JavaScript has a convenient `window.location` property you can use.

Note: The Javascript `window` object corresponds to a web browser window.

## Syntax

An example of the syntax is shown below:

```javascript
window.location;
```

### Properties

If you type `window.location;` in the browsers JavaScript console and run it, it will return a location object listing all properties and methods.

```javascript
window.location;

// returns the 'Location' object
Location {
  hash: "",
  host: "devdocs.io",
  hostname: "devdocs.io",
  href: "http://devdocs.io/dom/window/location",
  origin: "http://devdocs.io",
  pathname: "/dom/window/location",
  port: "",
  protocol: "http:",
  reload: function reload(),
  replace: function(),
  search: "",
  assign: function()
}
```

#### hash

The `hash` property sets or returns the anchor part of a URL, including the hash sign (#). Hash is the part of the URL from the # on (or an empty string if there is no #).

```javascript
window.location.href;
// full url "https://www.google.com/webhp?sourceid=chrome-instant&ion=1&espv=2&ie=UTF-8#q=window.location.hash"

window.location.hash;
// hash "#q=window.location.hash"
```

#### host

Sets or returns the site name and includes the port number.

```javascript
window.location.host;
// "example.org:8888"
```

#### hostname

Sets or returns the site name only.

```javascript
window.location.hostname;
// "example.org"
```

#### href

Sets or returns the site url.

```javascript
window.location.href;
// "http://encyclopedia.moderndeveloper.com/"
```

#### origin

Returns the protocol, hostname and port number of a URL.

```javascript
window.location.origin;
// "http://encyclopedia.moderndeveloper.com:1234"
```

#### pathname

Sets or returns the path of the current url.

```javascript
window.location.pathname;
// "/directory/file.php"
```

#### port

Sets or returns the port number of a url.

```javascript
window.location.port;
// "1234"
```

#### protocol

Sets or returns the protocol of a url.

```javascript
window.location.protocol;
// "http:"
```

#### search

Sets or returns the querystring part of a URL.

```javascript
window.location.search;
// "?q=how+to+program&oq=how+to+program&aqs=chrome..69i57.7935j0j1&sourceid=chrome&ie=UTF-8"
```

### Methods

#### reload

Reloads the current document.  
Note: By default this method reloads from the cache. If you wish to reload from the server, set the parameter to true.

```javascript
window.location.reload(true);
```

#### replace

Replaces the current document with new one.  
Note: This method does not allow you to use the back button once the document is loaded. Instead use the `location.assign()` method if you want to navigate back to the original document.

```javascript
window.location.replace(`newUrl`);
```

#### assign

Loads a new document.

```javascript
window.location.assign("http://encyclopedia.moderndeveloper.com/");
```

## Example 1

In this example the `href` value is set to point to an anchor in the page.

```javascript
location.href = "#article";
```

## Example 2

This example shows a function that takes a url string as a parameter and executes the `location.assign()` property with the new url.

```javascript
var assignLoc = function assignLoc(url) {
  location.assign(url);
}
```

## Browser Support

The `window.location` property is supported by all modern web browsers.

Google Chrome | Internet Explorer | Microsoft Edge | Firefox | Safari | Opera
--- | --- | --- | --- | --- | ---
Supported | Supported | Supported | Supported | Supported | Supported

## Special Notes

The `window.location` object can be written without the window prefix.

```javascript
location.protocol;
// "http:"
```