# margin-bottom

A CSS property.

The `margin-bottom` property sets the bottom margin of an element.

## Syntax

An example of the CSS syntax is shown below:

```css
.box {
  margin-bottom: <length | percentage | auto | initial | inherit>;
}
```

## Values

#### length

Specifies a fixed width in `px`, `em`, `pt`, and other *length units.* The default value is 0.

#### percentage

Specifies a `bottom-margin` percentage width relative to its parent element.

#### auto

You can calculate the bottom margin automatically by setting it to `auto`. Typically it is used to center an element within its container.  

As the element takes up the specified width, the remaining space will be split equally between the left and right margins.

#### initial

Sets the property to its default value.

#### inherit

Inherits this property from its parent element.

## Example 1

Sets the bottom margin to 15px.

```css
.box {
  margin-bottom: 15px; 
} 
```

## Example 2

Negative values are accepted also.

```css
.box {
  margin-bottom: -1.5em;
}
```

## Browser Support

The `margin-bottom` property is supported by all modern web browsers.

Google Chrome | Internet Explorer | Microsoft Edge | Firefox | Safari | Opera
--- | --- | --- | --- | --- | ---
Supported | Supported | Supported | Supported | Supported | Supported 

## Special Notes

#### Margin Collapse

When you have a scenario that consist of two vertical margins stacked on top of one another, the browser will cancel out the smaller margin and leave the larger one. This behavior is known as margin collapsing. For example:

```css
.box1 {
  margin-bottom: 20px;
}

.box2 {
  margin-top: 30px;
}
```

In the code above we have two boxes stacked with a bottom margin of 20px and a top margin of 30px. So you would think that 20px + 30px = 50px right? Well that doesn't happen. The browser picks the largest margin and runs with that only. In this case it would be 30px. The 20px margin would be cancelled out. Margins of floating and absolutely positioned elements never collapse.