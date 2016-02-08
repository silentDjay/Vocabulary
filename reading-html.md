## `<html>`

Referred to as the `root element`, all other html elements must live within this one. The last element of an HTML document must close out this tag with </html>.

Syntax: <html></html>

* _parents_: none
* _content_: _only_ [`<head>`](#head) and [`<body>`](#body)
* _display_: none - only the elements within the `<body>` tag display.

### Attributes

* `manifest` -- Specifies the URI of a resource manifest indicating resources that should be cached locally
* `version` -- Specifies the version of the HTML Document Type Definition that governs the current document. Really, though, this element is useless and made redundant by the `<!DOCTYPE>`declaration (see below).

. . .

## `<div>`

A generic page division that should typically only be used if no other, more semantic choice is appropriate.

Syntax: <div class="divClass"></div>

* _parents_: anything that accepts [Flow Content][1]
* _content_: any [Flow Content][1]
* _display_: `block`

### Attributes

* `class` -- a space-separated list of category names
* `id` -- an intradocument-unique declaration for styling purposes
* all other [global attributes][2]

. . .

## `<!-- -->`

This is an HTML comment. Anything inside the bracket will appear in the code but will not show up (or impact in any way) the content of the rendered HTML. It is used to make code more human-readable and less inscrutable.

Syntax: <!--THIS IS A USEFUL COMMENT-->

* _parents_: A comment can live outside of or within any html tag
* _content_: any text
* _display_: none - comments only appear witihn the source code

### Attributes

* whatever you feel like

## `<!DOCTYPE>`

This must be the very first element of an HTML file. It tells the web browser, or whatever is rendering your HTML, what kind (version) of HTML this file contains, and accordingly what kind of HTML the browser should look for. This is a declaration, not a tag, as in it _declares_ the document's type.

Syntax: <!DOCTYPE html>

* _parents_: none
* _content_: only [`<html>`](#html)
* _display_: none - this is not a tag and does not contain any renderable content

### Attributes

* none

. . .

## `<head>`

One of the very first tags in every HTML file. The contents of the head do not display on the page when rendered.  Within the <head>, you will usually find a [`<link>`](#link) to a CSS stylesheet, as well as to any remotely hosted fonts, icon repositories, or CSS reset tools. It can also contain a declaration of what character set is used within the html document.

Syntax: <head></head>

* _parents_: [`<html>`](#html)
* _content_: <link>(s)
* _display_: Nothing within this tag displays on the page.

### Attributes

* `profile` -- The URIs of one or more metadata profiles, separated by white space.

. . .

## `<body>`

This section of the HTML document contains the content that will be rendered in the browser or other application and styled by the associated CSS file. It must be the second element of an html document, after [`<html>`](#html). There can be only one <body> tag within an html document.

Syntax: <body></body>

* _parents_: <html>, <mask>
* _content_: any [Flow Content][1]
* _display_: one huge `block`

### Attributes

* a lot of them, including all [global attributes][2]

. . .

## `<a>`

Stands for 'anchor', and is used to house a link embedded within the contents of the page. This is one of the most common inline element tags.

Syntax: <a href="[link redirect destination]">[displayContent]</a>

* _parents_: anything that accepts [Flow Content][1], which is apparently a lot of things.
* _content_: any [Flow Content][1], palpable content (WTF?)
* _display_: `inline`

### Attributes

* `class` -- a space-separated list of category names
* `href` -- 'hypertext reference' - defines the location where the link should redirect the user if they click on it

. . .

## `<p>`

Stands for 'paragraph'; automatically starts on a new line and the following element starts on a new line.

Syntax: <p>This is the first paragraph of text. This is the first paragraph of text.
  This is the first paragraph of text. This is the first paragraph of text.</p>

* _parents_: anything that accepts [Flow Content][1]
* _content_: any [Flow ][1], palpable content (WTF?)
* _display_: `block`

### Attributes

* a lot of them, including all [global attributes][2]

. . .

## `<img>`

Used for incorporating images into your HTML.

syntax: <img class="Trangle" src="[filepath]" alt="Description of image contents">

* _parents_: anything that accepts [Flow Content][1]
* _content_:  
* _display_: `block`

### Attributes

* `class` -- a space-separated list of category names
* `src` -- path to local (or remotely hosted) image file to display with tag
* `alt` -- _alternate_ text to image. Concisely describes contents of image; typically displays upon hover over image.

. . .

## `<span>`

A tag which can envelop a text element within other elements/tags/etc.

Syntax: 

* _parents_: anything that accepts [Flow Content][1], which is apparently a lot of things.
* _content_: any [Flow Content][1], palpable content (WTF?)
* _display_: `inline`

### Attributes

* `class` -- a space-separated list of category names
* . . .

. . .

###### Footnotes

[1](https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/Content_categories#Flow_content)
[2](https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes)
[3](https://en.wikipedia.org/wiki/HTML_element)
