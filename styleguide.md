#Style Guide
The key words "MUST", "MUST NOT", "REQUIRED", "SHALL", "SHALL NOT", "SHOULD", "SHOULD NOT", "RECOMMENDED", "MAY", and "OPTIONAL" in this document are to be interpreted as described in [RFC 2119](http://www.ietf.org/rfc/rfc2119.txt).

Adapted from:
https://github.com/styleguide
http://google-styleguide.googlecode.com/svn/trunk/htmlcssguide.xml
http://codex.wordpress.org/WordPress_Coding_Standards

##HTML
####Doctype
For simplicity and maximum compatibility, use the HTML5 doctype.  This tag is REQUIRED.
```html
<!DOCTYPE html>
```


####Charset
Make sure your text editor is using UTF-8 as the character encoding.  Do not use a byte order mark (BOM).
Specify the character set in HTML documents using the charset meta tag.  This tag is REQUIRED.
```html
<meta charset="utf-8">
```


####Formatting
#####New Lines and Indentation
Use a new line for every block level element.  Indent each new line by 2 spaces.  The author MUST NOT mix tabs and spaces.
```html
<blockquote>
  <p><em>Lorem</em> ipsum dolor sit amet.</p>
</blockquote>
```

#####Capitalization
Use only lowercase in element names, attributes, attribute values, selectors, properties, and property values.  The only exception to this is text or strings.
```html
<img src="foo.png" alt="Bar">
```

#####Attributes
For HTML attribute values Use double quotes ("") instead of single quotes ('').
Omit `type` attributes from style sheet and script declarations.
```html
<link rel="stylesheet" href="foo.css">
```
```html
<script src="bar.js"></script>
```


####Accessibility
#####Alt attribute
Use meaningful alternate text on all non-decorative images, videos, and animated `canvas` objects.
```html
<img src="logo.png" alt="Foo Bar Incorporated">
```


##CSS
###ID attribute
Avoid using ID attributes as CSS selectors.

###Shorthand
Use shorthand properties whenever possible.
```css
h1{
  font: 1.5em/1.2 Helvetica, Arial, sans-serif;
}
```

Use 3 character hexadecimal notation whenever possible.
```css
body {
  color: #F00;
}
```


###Zero value unit
Omit unit specification after "0" values unless required.
```css
.foo {
  margin: 0;
}
```

###Line-height
Do not specify a unit when declaring line height.
```css
h2 {
  line-height: 1.2;
}
```

###Formatting
Use a semicolon after every property declaration.
Use a space after every property name's colon.
Start a new line for each selector and declaration.
Leave a blank line between blocks of rules.
```css
.foo,
.bar {
  margin: 0;
  padding: 0;
}

.baz {
  margin: 0 auto;
}
```