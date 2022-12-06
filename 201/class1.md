# README.md

## Read Assignment 1 Notes git clone

**Computers connected to the internet are called clients and servers.**

* Clients are the typical web user's internet-connected devices for example, your computer connected to your Wi-Fi, or your phone connected to your mobile network and web-accessing software available on those devices usually a web browser like Firefox or Chrome.

* Servers are computers that store webpages, sites, or apps. When a client device wants to access a webpage, a copy of the webpage is downloaded from the server onto the client machine to be displayed in the user's

* When browsers send requests to servers for HTML files, those HTML files often contain *link* elements referencing external CSS stylesheets and *script* elements referencing external JavaScript scripts. It's important to know the order in which those files are parsed by the browser as the browser loads the page:

* The browser parses the HTML file first, and that leads to the browser recognizing any *link* -element references to external CSS stylesheets and any *script* -element references to scripts.

* As the browser parses the HTML, it sends requests back to the server for any CSS files it has found from *link* elements, and any JavaScript files it has found from *script* elements, and from those, then parses the CSS and JavaScript.

* The browser generates an in-memory DOM tree from the parsed HTML, generates an in-memory CSSOM structure from the parsed CSS, and compiles and executes the parsed JavaScript.

* As the browser builds the DOM tree and applies the styles from the CSSOM tree and executes the JavaScript, a visual representation of the page is painted to the screen, and the user sees the page content and can begin to interact with it.

## Images in HTML

In order to put a simple image on a web page, we use the *img* element. This is a void element -meaning, it cannot have any child content and cannot have an end tag that requires two attributes to be useful: src and alt. The src attribute contains a URL pointing to the image you want to embed in the page. As with the href attribute for *a* elements, the src attribute can be a relative URL or an absolute URL. Without a src attribute, an img element has no image to load.

## Strings — the basics

Strings are dealt with similarly to numbers at first glance, but when you dig deeper you'll start to see some notable differences. Let's start by entering some basic lines into the browser developer console to familiarize ourselves.

## Creating a string

To start with, enter the following lines:const string = "The revolution will not be televised.";
console.log(string);
The following will work if you previously defined the variable string — try it now:
const badString = string;
console.log(badString);

## Types of numbers

In programming, even the humble decimal number system that we all know so well is more complicated than you might think. We use different terms to describe different types of decimal numbers, for example:
Integers are floating-point numbers without a fraction. They can either be positive or negative, e.g. 10, 400, or -5.

* Floating point numbers (floats) have decimal points and decimal places, for example 12.5, and 56.7786543.

* Doubles are a specific type of floating point number that have greater precision than standard floating point numbers (meaning that they are accurate to a greater number of decimal places).

## Converting To Number Data Types

Sometimes you might end up with a number that is stored as a string type, which makes it difficult to perform calculations with it. This most commonly happens when data is entered into a form input, and the input type is text. There is a way to solve this problem — passing the string value into the Number() constructor to return a number version of the same value.
For example, try typing these lines into your console:
let myNumber = "74";
myNumber += 3;
Copy to Clipboard

You end up with the result 743, not 77, because myNumber is actually defined as a string. You can test this by typing in the following:
typeof myNumber;
Copy to Clipboard

To fix the calculation, you can do this:
let myNumber = "74";
myNumber = Number(myNumber) + 3;
Copy to Clipboard

The result is then 77, as initially expected.

Arithmetic operators
Arithmetic operators are the basic operators that we use to do sums in JavaScript:

## What is a variable? 
A variable is a container for a value, like a number we might use in a sum, or a string that we might use as part of a sentence.
Variable example
Let's look at a simple example:

* <button id="button_A">Press me</button>

<h3 id="heading_A"></h3>
Copy to Clipboard

const buttonA = document.querySelector('#button_A');
const headingA = document.querySelector('#heading_A');

buttonA.onclick = () => {
  const name = prompt('What is your name?');
  alert(`Hello ${name}, nice to see you!`);
  headingA.textContent = `Welcome ${name}`;
}
Copy to Clipboard

In this example pressing the button runs some code. The first line pops a box up on the screen that asks the reader to enter their name, and then stores the value in a variable. The second line displays a welcome message that includes their name, taken from the variable value and the third line displays that name on the page.

## Attributes

Elements can also have attributes. Attributes look like this:

Attributes contain extra information about the element that won't appear in the content. In this example, the class attribute is an identifying name used to target the element with style information.

An attribute should have:

* A space between it and the element name. (For an element with more than one attribute, the attributes should be separated by spaces too.)

* The attribute name, followed by an equal sign.

* An attribute value, wrapped with opening and closing quote marks.

* Active learning: Adding attributes to an element

Another example of an element is *a*. This stands for anchor. An anchor can make the text it encloses into a hyperlink. Anchors can take a number of attributes, but several are as follows:
href
This attribute's value specifies the web address for the link. For example: href="https://www.mozilla.org/".

## Title

The title attribute specifies extra information about the link, such as a description of the page that is being linked to. For example, title="The Mozilla homepage". This appears as a tooltip when a cursor hovers over the element.

## Target

The target attribute specifies the browsing context used to display the link. For example, target="_blank" will display the link in a new tab. If you want to display the linked content in the current tab, just omit this attribute.

## Anatomy of an HTML element

The anatomy of our element is:
The opening tag: This consists of the name of the element (in this example, p for paragraph), wrapped in opening and closing angle brackets. This opening tag marks where the element begins or starts to take effect. In this example, it precedes the start of the paragraph text.

The content: This is the content of the element. In this example, it is the paragraph text.

The closing tag: This is the same as the opening tag, except that it includes a forward slash before the element name. This marks where the element ends. Failing to include a closing tag is a common beginner error that can produce peculiar results.

The element is the opening tag, followed by content, followed by the closing tag.

## Active learning: creating your first HTML element

Edit the line below in the "Editable code" area by wrapping it with the tags *em* and </em>. To open the element, put the opening tag *em* at the start of the line. To close the element, put the closing tag </em> at the end of the line. Doing this should give the line italic text formatting! See your changes update live in the Output area.
If you make a mistake, you can clear your work using the Reset button. If you get really stuck, press the Show solution button to see the answer.

**Article vs Section**

*Article* encloses a block of related content that makes sense on its own without the rest of the page (e.g., a single blog post).
*section* is similar to *article*, but it is more for grouping together a single part of the page that constitutes one single piece of functionality (e.g., a mini map, or a set of article headlines and summaries), or a theme.

Headers and footers are elements a typical website might need

**Meta Data**

The head of an HTML document is the part that is not displayed in the web browser when the page is loaded. It contains information such as the page *title*, links to CSS (if you choose to style your HTML content with CSS), links to custom favicons, and other metadata (data about the HTML, such as the author, and important keywords that describe the document). Web browsers use information contained in the head to render the HTML

**Metadata:**

The *meta* element
Metadata is data that describes data, and HTML has an "official" way of adding metadata to a document — the *meta* element. Of course, the other stuff we are talking about in this article could also be thought of as metadata too. There are a lot of different types of *meta* elements that can be included in your page's *head*, but we won't try to explain them all at this stage, as it would just get too confusing. Instead, we'll explain a few things that you might commonly see, just to give you an idea.
Specifying your document's character encoding
In the example we saw above, this line was included:
<meta charset="utf-8" />
document correctly. In this article we'll cover all of the above and more, in order to give you a good basis for working with markup.

**The first step to building a website**
have a vision of what you want and how to get there. Once you have that clear vision, you need to decide how and when to do it. Break down big tasks into small, actionable steps. And those small steps will add up to great achievements.

*First question to answer when building a website is What matters is to have a vision of what you want and how to get there. Once you have that clear vision, you need to decide how and when to do it. Break down big tasks into small, actionable steps. And those small steps will add up to great achievements.*

## Semantics

1. This will render it to look like a top level heading, but it has no semantic value, so it will not get any extra benefits as described above. It is therefore a good idea to use the right HTML element for the right job.
2. HTML should be coded to represent the data that will be populated and not based on its default presentation styling. Presentation (how it should look), is the sole responsibility of CSS.

## Semantics Tags

*Benefits from writing semantic markup are as follows:
Search engines will consider its contents as important keywords to influence the page's search rankings (see SEO)

Screen readers can use it as a signpost to help visually impaired users navigate a page

Finding blocks of meaningful code is significantly easier than searching through endless divs with or without semantic or namespaced classes

Suggests to the developer the type of data that will be populated
Semantic naming mirrors proper custom element/component naming*

## Things I want to know more about

## Explained

HTML is the markup language that we use to structure and give meaning to our web content, for example defining paragraphs, headings, and data tables, or embedding images and videos in the page.

* CSS is a language of style rules that we use to apply styling to our HTML content, for example setting background colors and fonts, and laying out our content in multiple columns.
* JavaScript is a scripting language that enables you to create dynamically updating content, control multimedia, animate images, and pretty much everything else. (Okay, not everything, but it is amazing what you can achieve with a few lines of JavaScript code.)

## Add JavaScript to HTML

* JavaScript is applied to your HTML page in a similar manner to CSS. Whereas CSS uses *link* elements to apply external stylesheets and *style* elements to apply internal stylesheets to HTML, JavaScript only needs one friend in the world of HTML — the *script* element.
