#Style Guide
The key words "MUST", "MUST NOT", "REQUIRED", "SHALL", "SHALL NOT", "SHOULD", "SHOULD NOT", "RECOMMENDED", "MAY", and "OPTIONAL" in this document are to be interpreted as described in [RFC 2119](http://www.ietf.org/rfc/rfc2119.txt).

##Markup

####Doctype
For simplicity and maximum compatibility, use the HTML5 doctype.  This tag is REQUIRED.
```html
<!DOCTYPE html>
`

####Charset
Make sure your text editor is using UTF-8 as the character encoding.  Do not use a byte order mark (BOM).
Specify the character set in HTML documents using the charset meta tag.  This tag is REQUIRED.
```html
<meta charset="utf-8">
`

####Formatting

#####Indentation
Indent each new line by 2 spaces.  The author MUST NOT mix tabs and spaces.
```html
    <ul>
      <li>Foo</li>
      <li>Bar</li>
    </ul>
`