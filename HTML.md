#### HTML Questions:

* What does a `doctype` do?
  - http://html.com/tags/doctype/

* What's the difference between full standards mode, almost standards mode and quirks mode?
  - https://developer.mozilla.org/en-US/docs/Quirks_Mode_and_Standards_Mode
  - https://hsivonen.fi/doctype/

* What's the difference between HTML and XHTML?
  - http://www.webstandards.org/learn/articles/askw3c/oct2003/
  - https://developer.mozilla.org/en-US/docs/Glossary/XHTML

  - Stack Overflow (use with caution)

    - XHTML is based on XML, and thus requires the source to be well-formed. Since XHTML is more strict than HTML, less pre-processing is needed by the rendering engine. XHTML should be served as application/xhtml+xml for you to take advantage of the benefits, otherwise XHTML will be treated as ordinary HTML. Serving it as 'application/xhtml+xml' is not common on the web due to Internet Explorer, which cannot handle XHTML.

    - The Extensible Hypertext Markup Language, or XHTML, is a markup language that has the same depth of expression as HTML, but also conforms to XML syntax. XHTML is "the modern version of HTML 4".

* Are there any problems with serving pages as `application/xhtml+xml`?
  -

* How do you serve a page with content in multiple languages?
  - https://www.w3.org/International/questions/qa-html-language-declarations

* What kind of things must you be wary of when design or developing for multilingual sites?


* What are `data-` attributes good for?
  - https://developer.mozilla.org/en-US/docs/Learn/HTML/Howto/Use_data_attributes
  - HTML5 is designed with extensibility in mind for data that should be associated with a particular element but need not have any defined meaning. data-* attributes allow us to store extra information on standard, semantic HTML elements without other hacks such as non-standard attributes, extra properties on DOM, or Node.setUserData(). HTML syntax: The syntax is simple. Any attribute on any element whose attribute name starts with data- is a data attribute. Say you have an article and you want to store some extra information that doesn’t have any visual representation.
  - The data-* attributes gives us the ability to embed custom data attributes on all HTML elements. The stored (custom) data can then be used in the page's JavaScript to create a more engaging user experience (without any Ajax calls or server-side database queries). ... The attribute value can be any string.

* Consider HTML5 as an open web platform. What are the building blocks of HTML5?
* Describe the difference between a `cookie`, `sessionStorage` and `localStorage`.
  - https://developer.mozilla.org/en-US/docs/Web/API/Web_Storage_API
  - Quora:
    - sessionStorage, localStorage and Cookies all are used to store data on the client side. Each one has its own storage and expiration limit.

    - localStorage: stores data with no expiration date, and gets cleared only through JavaScript, or clearing the Browser Cache / Locally Stored Data

    - sessionStorage: similar to localStorage but expires when the browser closes (not the tab).

    - Cookie: stores data that has to be sent back to the server with subsequent requests. Its expiration varies based on the type and the expiration duration can be set from either server-side or client-side (normally from server-side). Cookies are primarily for server-side reading (can also be read on client-side), localStorage and sessionStorage can only be read on client-side.

* Describe the difference between `<script>`, `<script async>` and `<script defer>`.
  - https://developer.mozilla.org/en-US/docs/Web/HTML/Element/script
  - async HTML5: Set this Boolean attribute to indicate that the browser should, if possible, execute the script asynchronously. It has no effect on inline scripts (i.e., scripts that don't have the src attribute). See Browser compatibility for notes on browser support. See also Async scripts for asm.js.
  - defer: This Boolean attribute is set to indicate to a browser that the script is meant to be executed after the document has been parsed, but before firing DOMContentLoaded. The defer attribute should only be used on external scripts.

* Why is it generally a good idea to position CSS `<link>`s between `<head></head>` and JS `<script>`s just before `</body>`? Do you know any exceptions?
  - This loads CSS before page is rendered, reason not to, accessibility? If you put it after, does this mean page has to load twice?

* What is progressive rendering?
  - http://www.ebaytechblog.com/2014/12/08/async-fragments-rediscovering-progressive-html-rendering-with-marko/
  -  https://medium.com/ben-and-dion/progressive-rendering-a-killer-and-under-appreciated-feature-of-the-web-97c789b608c1#.3luhkyr0d
  - https://en.wikipedia.org/wiki/Lazy_loading
  - https://developers.google.com/speed/docs/insights/PrioritizeVisibleContent

* Have you used different HTML templating languages before?
  - Handlebars
  - Angular
  - List of top 2016 templating languages: https://colorlib.com/wp/top-templating-engines-for-javascript/
