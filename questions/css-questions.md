# CSS Questions:

* What is CSS selector specificity and how does it work?

Inline styles - An inline style is attached directly to the element to be styled. Example: <h1 style="color: #ffffff;">.

IDs - An ID is a unique identifier for the page elements, such as #navbar.

Classes, attributes and pseudo-classes - This category includes .classes, [attributes] and pseudo-classes such as :hover, :focus etc.

Elements and pseudo-elements - This category includes element names and pseudo-elements, such as h1, div, :before and :after.

* What's the difference between "resetting" and "normalizing" CSS? Which would you choose, and why?

CSS resets aim to remove all built-in browser styling. Standard elements like H1-6, p, strong, em, et cetera end up looking exactly alike, having no decoration at all. You're then supposed to add all decoration yourself.

Normalize CSS aims to make built-in browser styling consistent across browsers. Elements like H1-6 will appear bold, larger et cetera in a consistent way across browsers. You're then supposed to add only the difference in decoration your design needs.



* Describe Floats and how they work.

The float CSS property specifies that an element should be placed along the left or right side of its container, allowing text and inline elements to wrap around it.


* Describe z-index and how stacking context is formed.

The stacking context is a three-dimensional conceptualization of HTML elements along an imaginary z-axis relative to the user, who is assumed to be facing the viewport or the webpage. HTML elements occupy this space in priority order based on element attributes.


* Describe BFC(Block Formatting Context) and how it works.

A block formatting context is a part of a visual CSS rendering of a Web page. It is the region in which the layout of block boxes occurs and in which floats interact with other elements.


* What are the various clearing techniques and which is appropriate for what context?


* How would you approach fixing browser-specific styling issues?


Always build responsive layouts.
Check features of HTML5 and CSS3 on caniuse.com to see what browser support there is for something new I want to use and avoid things that have sketchy support at this time.
Develop all of the views at the same time and test across browsers and operating systems as I go to avoid getting something that looks nice in my favorite browser, but breaks in other places that I then have to fix later with the potential of having to start from scratch.
Realize that we don’t have to make the display on every browser exactly identical as long as what we make looks good in each browser. Graceful degradation means that your design is able to fall back to a decent, but simplified, version of the layout rather than just looking broken in browsers that don’t support certain features of HTML or CSS.
Keep up-to-date on what browsers and systems my target-audience is using, either by looking at Google Analytics on the existing site I’m replacing for the client, or periodically checking Stat Counter.
Use BrowserStack for more intense cross-browser testing.
Use the knowledge and experience I’ve gained from my years in web development to know in advance what to avoid or what to do to make something work in all the browsers.


* How do you serve your pages for feature-constrained browsers?
  * What techniques/processes do you use?
  
  
* What are the different ways to visually hide content (and make it available only for screen readers)?

visibility: hidden; and/or display:none;

width:0px, height:0px or other 0 pixel sizing techniques

text-indent: -10000px;




* Have you ever used a grid system, and if so, what do you prefer?

Bootstrap Grid System


* Have you used or implemented media queries or mobile specific layouts/CSS?

Media query is a CSS technique introduced in CSS3.

It uses the @media rule to include a block of CSS properties only if a certain condition is true.


* Are you familiar with styling SVG?


* Can you give an example of an `@media` property other than `screen`?
* What are some of the "gotchas" for writing efficient CSS?




* What are the advantages/disadvantages of using CSS preprocessors?

A CSS preprocessor is a program that lets you generate CSS from the preprocessor's own unique syntax. There are many CSS preprocessors to choose from, however most CSS preprocessors will add some features that don't exist in pure CSS, such as mixin, nesting selector, inheritance selector, and so on




  * Describe what you like and dislike about the CSS preprocessors you have used.
* How would you implement a web design comp that uses non-standard fonts?
* Explain how a browser determines what elements match a CSS selector.
* Describe pseudo-elements and discuss what they are used for.
* Explain your understanding of the box model and how you would tell the browser in CSS to render your layout in different box models.
* What does ```* { box-sizing: border-box; }``` do? What are its advantages?
* What is the CSS `display` property and can you give a few examples of its use?
* What's the difference between inline and inline-block?
* What's the difference between a relative, fixed, absolute and statically positioned element?
* What existing CSS frameworks have you used locally, or in production? How would you change/improve them?
* Have you played around with the new CSS Flexbox or Grid specs?
* Can you explain the difference between coding a web site to be responsive versus using a mobile-first strategy?
* Have you ever worked with retina graphics? If so, when and what techniques did you use?
* Is there any reason you'd want to use `translate()` instead of *absolute positioning*, or vice-versa? And why?
