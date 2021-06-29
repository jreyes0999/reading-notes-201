# Wireframe
  * Wireframing allows the UX design team to know where every bit of information will go and positioning buttons, menus, and everything else before starting to code. 
  * Made by hand - Wireframes drawn with paper and a pencil, or at a whiteboard, have the advantage of looking and being very easy to change. With the help of paper-prototypes, you can test with end users at every stage of ideation and design. Changes at these stages are much easier—and therefore cheaper.
  * Using using software like **InVision** or **Balsamiq**. Free software: **UXPin**, **InVision**, and **Wireframe.cc**.
    * Wireframe > Interactive Prototype > Visual > Design
    * Sketch > Code
    * Sketch > Wireframe > Hi-Def Wireframe > Visual > Code
    * Sketch > Wireframe > Visual > Code

## Wireframe Steps
   1. Do your research.
   2. Prepare your research for quick reference
   3. Make sure you have your user flow mapped out
   4. Draft, don’t draw. Sketch, don’t illustrate
   5. Add some detail and get testing
   6. Start turning your wireframes into prototypes

## Key Principles for a Good Wireframe
   * Clarity - Answers questions like, what the page is, what the user can do there, and if it satisfies their needs. 
   * Confidence - Ease of navigation, clear calls-to-action, and using familiar positioning and processes.
   * Simplicity - You want your users to be able to find their way through your site with as little extra ‘fluff’ as possible

# HTML (**H**yper**t**ext **M**arkup **L**anguage)
 * "Hypertext" refers to links that connect web pages to one another, either within a single website or between websites. Links are a fundamental aspect of the Web. By uploading content to the Internet and linking it to pages created by other people, you become an active participant in the World Wide Web.

## What is HTML?
* HTML is a markup language that defines the structure of your content. HTML consists of a series of elements, which you use to enclose, or wrap, different parts of the content to make it appear a certain way, or act a certain way. The enclosing tags can make a word or image hyperlink to somewhere else, can italicize words, can make the font bigger or smaller, and so on
  * HTML uses "markup" to annotate text, images, and other content for display in a Web browser. HTML markup includes special "elements" such as <head>, <title>, <body>, <header>, <footer>, <article>, <section>, <p>, <div>, <span>, <img>, <aside>, <audio>, <canvas>, <datalist>, <details>, <embed>, <nav>, <output>, <progress>, <video>, <ul>, <ol>, <li> and many others.
    
### HMTL Basics
  * An HTML element is set off from other text in a document by "tags", which consist of the element name surrounded by "<" and ">".  The name of an element inside a tag is case insensitive. That is, it can be written in uppercase, lowercase, or a mixture. For example, the <title> tag can be written as <Title>, <TITLE>, or in any other way.
    * The opening tag: This consists of the name of the element, wrapped in opening and closing angle brackets. This states where the element begins or starts to take effect.
      * The closing tag: This is the same as the opening tag, except that it includes a forward slash before the element name. This states where the element ends; <p> </p> Failing to add a closing tag is one of the standard beginner errors and can lead to strange results.
        * The content: This is the content of the element.
        * The element: The opening tag, the closing tag, and the content together comprise the element.
          * **Elements can also have attributes** and should have the following:
            * A space between it and the element name (or the previous attribute, if the element already has one or more attributes).
            * The attribute name followed by an equal sign.
            * The attribute value wrapped by opening and closing quotation marks. 

## Anatomy of an HTML document
  * !DOCTYPE html — doctype. Needed to make your document behave correctly. 
  * html | /html — This element wraps all the content on the entire page and is sometimes known as the root element.
  * head | /head — This element acts as a container for all the stuff you want to include on the HTML page that isn't the content you are showing to your page's viewers. This includes things like keywords and a page description that you want to appear in search results, CSS to style our content, character set declarations, and more.
  * meta charset="utf-8" — This element sets the character set your document should use to UTF-8 which includes most characters from the vast majority of written languages. Essentially, it can now handle any textual content you might put on it. There is no reason not to set this and it can help avoid some problems later on.
  * title | /title — This sets the title of your page, which is the title that appears in the browser tab the page is loaded in. It is also used to describe the page when you bookmark/favorite it.
  * body | /body — This contains all the content that you want to show to web users when they visit your page, whether that's text, images, videos, games, playable audio tracks, or whatever else.

### Headings
  * Heading elements allow you to specify that certain parts of your content are headings — or subheadings. In the same way that a book has the main title, chapter titles, and subtitles, an HTML document can too. HTML contains 6 heading levels, <h1>–<h6>, although you'll commonly only use 3 to 4 at most:
    * "<h1>My main title</h1>"
    * "<h2>My top level heading</h2>"
    * "<h3>My subheading</h3>"
    * "<h4>My sub-subheading</h4>"

### Lists
    1. Unordered lists are for lists where the order of the items doesn't matter, such as a shopping list. These are wrapped in a <ul> element.
    2. Ordered lists are for lists where the order of the items does matter, such as a recipe. These are wrapped in an <ol> element.
Example: 
`<ul>`
  `<li>``</li>`
  `<li>``</li>`
  `<li>``</li>`
`</ul>`

### Links
  *  To add a link, we need to use a simple element — `<a>` — "a" being the short form for "anchor". To make text within your paragraph into a link, follow these steps:
Example: `"<a href="link">text</a>"` "<a href="https://youtube.com">YouTube</a>"

# Semantics
  * In programming, Semantics refers to the meaning of a piece of code — for example "what effect does running that line of JavaScript have?", or "what purpose or role does that HTML element have" (rather than "what does it look like?".)
## Semantics in JavaScript
  * In JavaScript, consider a function that takes a string parameter, and returns an "<li>" element with that string as its textContent. Would you need to look at the code to understand what the function did if it was called build('Peach'), or createLiWithContent('Peach')?
## Semantics in CSS
  * In CSS, consider styling a list with li elements representing different types of fruits. Would you know what part of the DOM is being selected with div > ul > li, or .fruits__item?
## Semantics in HTML
  * In HTML, for example, the `<h1>` element is a semantic element, which gives the text it wraps around the role (or meaning) of "a top level heading on your page." HTML should be coded to represent the data that will be populated and not based on its default presentation styling. Presentation (how it should look), is the sole responsibility of CSS.
### Benefits from Writing Semantic Markup
 * Search engines will consider its contents as important keywords to influence the page's search rankings.
 * Screen readers can use it as a signpost to help visually impaired users navigate a page
 * Finding blocks of meaningful code is significantly easier than searching through endless divs with or without semantic or namespaced classes.
 * Suggests to the developer the type of data that will be populated.
 * Semantic naming mirrors proper custom element/component naming.
### Semantic elements
These are *some* of the roughly 100 semantic elements available: 
  * "<article>"
  * "<aside>"
  * "<footer>"
  * "<header>"
  * "<main>"
  * "<nav>"
   
