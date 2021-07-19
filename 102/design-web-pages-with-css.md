# What is CSS?
* CSS (**C**ascading **S**tyle **S**heets) allows you to create great-looking web pages.

## What is CSS for? 
* CSS can be used for very basic document text styling — for example changing the color and size of headings and links. It can be used to create layout — for example turning a single column of text into a layout with a main content area and a sidebar for related information. It can even be used for effects such as animation.

## CSS Syntax
* CSS is a rule-based language — you define rules specifying groups of styles that should be applied to particular elements or groups of elements on your web page.
    * The rule opens with a selector . This selects the HTML element that we are going to style.
* We then have a set of curly braces { }. Inside those will be one or more declarations, which take the form of property and value pairs. Each pair specifies a property of the element(s) we are selecting, then a value that we'd like to give the property.Before the colon, we have the property, and after the colon, the value.

## 3 Ways to Insert CSS
* External CSS - With an external style sheet, you can change the look of an entire website by changing just one file! Each HTML page must include a reference to the external style sheet file inside the `<link>` element, inside the head section. An external style sheet can be written in any text editor, and must be saved with a .css extension.

```
<style>
    h1 {
        color: red;
        font-size: 5em;
}
</style>
```

* Internal CSS - An internal style sheet may be used if one single HTML page has a unique style. The internal style is defined inside the `<style>` element, inside the head section.

```
<link rel="stylesheet" href="style.css">
```
* Inline CSS - An inline style may be used to apply a unique style for a single element. To use inline styles, add the style attribute to the relevant element. The style attribute can contain any CSS property.

```
<p style="color: red; text-align:center;">
```

## CSS Color Property
* The color property specifies the color of text. 
* CSS Syntax: color: color|initial|inherit;
* Can be set with HEX, RGB, RGBA, HSL, and HSLA values. 

### Basic Selectors
* Universal selector `*, ns|*, *|*, |*`
* Type selector elementname
* Class selector .classname
* ID selector #idname
* Attribute selector [attr=value]

### CSS Tools: Reset CSS
* The goal of a reset stylesheet is to reduce browser inconsistencies in things like default line heights, margins and font sizes of headings, and so on. 
* The reset styles given here are intentionally very generic. There isn't any default color or background set for the body element, for example.
