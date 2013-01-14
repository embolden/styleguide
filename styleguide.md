#Style Guide
The key words "MUST", "MUST NOT", "REQUIRED", "SHALL", "SHALL NOT", "SHOULD", "SHOULD NOT", "RECOMMENDED", "MAY", and "OPTIONAL" in this document are to be interpreted as described in [RFC 2119](http://www.ietf.org/rfc/rfc2119.txt).

Adapted from:
- https://github.com/styleguide
- http://google-styleguide.googlecode.com/svn/trunk/htmlcssguide.xml
- http://codex.wordpress.org/WordPress_Coding_Standards

##HTML
####Doctype
The author MUST use the HTML5 doctype.  This ensures maximum accessibility, compatibility, support, and simplicity.
```html
<!DOCTYPE html>
```


####Encoding
The author MUST declare a character set for a document.  The RECOMMENDED encoding method is UTF-8.  The author SHOULD use the HTML5 meta tag.  Make sure that the chosen editor is using the UTF-8 without a byte order mark (BOM).
```html
<meta charset="utf-8">
```


####Formatting
#####New Lines and Indentation
The author MUST use a new line for every block line.  Each nested element MUST be indented 2 spaces.  The author MUST NOT mix tabs and spaces.
```html
<blockquote>
  <p><em>Lorem</em> ipsum dolor sit amet.</p>
</blockquote>
```

#####Capitalization
The author MUST use only lowercase letters for element names, attributes, attribute values, selectors, properties, and property values.  The only exception to this is text or strings.
```html
<img src="foo.png" alt="Bar">
```

#####Attributes
The author MUST use double quotes ("") instead of single quotes ('') for HTML attributes.
The author MUST omit `type` attributes from style sheet and script declarations.
```html
<link rel="stylesheet" href="foo.css">
```
```html
<script src="bar.js"></script>
```


####Accessibility
#####Alt attribute
The author MUST use meaningful alternate text on all non-decorative images, videos, and animated `canvas` objects.
```html
<img src="logo.png" alt="Foo Bar Incorporated">
```



##CSS
###ID attribute
The author SHOULD avoid using ID attributes as CSS selectors.


###Shorthand
The author SHOULD use shorthand properties whenever available.
```css
h1{
  font: 1.5em/1.2 Helvetica, Arial, sans-serif;
}
```


The author SHOULD use 3 character hexadecimal notation whenever possible.
```css
body {
  color: #F00;
}
```


###Zero value unit
The author SHOULD omit unit specification after "0" values.
```css
.foo {
  margin: 0;
}
```


###Line-height
The author SHOULD NOT specify a measurement unit when declaring line height.
```css
h2 {
  line-height: 1.2;
}
```


###Formatting
The author MUST use a semicolon after every property declaration.
The author MUST use a space after every property name's colon.
The author MUST start a new line for each selector and declaration.
The author MUST leave a blank line between blocks of rules.
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