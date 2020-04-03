## HTML Notes

# Process and Design (Chapter 18)

When creating a website you must conisder a few things:
* Who is this website for?
* Why will people be visiting your website?
    * What are the underlying motivations of visitors?
    * What are the specific goals of the visitors?
* What are your visitors trying to achieve?
* What information do your visitors need?
* How often will people visit your site?

After deciding what needs to appear on your website, you need to organize the information into sections or pages. This can be done using a **site map**.

* A **site map** is a diagram of the pages that will be used to structure the site. This shows how the pages will be grouped. 
* A **site map** usually begins with a homepage, and the other pages are compartmentalized into sections that are linked to the homepage.

* A **wirefram** is a simple sketch of the key information that needs to go on each page of a site. It shows the hierarchy of information and how much space it might require.

### Design

* Webpages contain a lot of content that need to be organized and prioritized.

* **Visual Hierarchy** refers to the order in which your eyes percieve what they see. It is created by adding **visual contrast** between items being displayed, the items with higher contrast are recognized and processed first. Visual hierarchy helps to get the visitor's attention on the important stuff using size, color, and style.
* Images create a high visual contrast and often attract the eye first.

* **Grouping** related pieces of information together can make a design easier to comprehend.

* **Navigation** helps people find where they want to go on your site and how your site works.

## Structure (Chapter 1)

* HTML uses **tags** (characters that sit within angled brackets) to give the information they surround meaning.
* Tags are often reffered to as elements.
* Tags usually come in pairs. The opening tag denotes the start of a piece of content, the closing tag denotes the end. 
* **Attribues** require a 
*name* and a *value*.
    * Name = wha5t kind of information you are supplying about the elements contents.
    * Value = the information or setting for the sttribute. Should be in double quotes.

## HTML5 Layout (Chapter 17)

* The `<div>` element is used to group together related elenments on the page.
* The class or id attributes indicate the role of the `<div>` element in the structure of the page.

### HTML5 Layout Elements:

* The `<header>` and `<footer>` elements can be used for:
    * The main header or footer that appears at the top or bottom of every page on the site.
    * A header or footer for an individual `<article>` or `<section>` within the page.
* The `<nav>` element is used to contain the major navigational blocks on the site such as the primary site navigation. 
* The `<article>` element acts as a container for any section of a page that could stand alone.
* The `<aside>` element has two purposes depending on whether it is inside an `<article>` element or not.
    * When the `<aside>` element is used inside a `<article>` element. it should contain info that is related to the article but not essential to its overall meaning. Ex.) a pullquote or glossary.
    * When the `<aside>` element is used outside of an `<article>`, it acts as a container for content that is related to the entire page. Ex.) links to other sections of the site or a search box.
* The `<section>` element groups related content together.
* The `<hgroup>` element groups together a set of one or more `<h1>` through `<h6>` elements so they are treated as a single heading.
* The `<figure>` element is used to contain any content that is referenced in the main flow of an article (not just images.) Examples of usage are images, videos, graphs, diagrams, code samples, and text that supports the main body of an article.
    * THe `<figure>` element should also contain a `<figcaption>` element which provides a text description for the content in the figure element.

## Extra Markup (Chapter 8)

* Because there are several versions of HTML, each web page should begin with a DOCTYPE declaration on top to tell what type it is.
* If you want to adda comment in the code that isn't visible in the user's browser use: `<!--comment goes here-->`
* The **id attribute** is used to uniquely identify an elemnt from other elements on the page. Its value should start with a letter or an underscore. The **id attribute** is known as a global attribute because it can be used on any element.
* The **class attribute** gives a way to identify several elements as being different from the other elements on the page. Its value should describe the class it belongs to.
* **Block Elements** are elemnts that will always appear to start on a new line in the browser window. Examples of block elements are: `<h1>`, `<p>`,`<ul>`, and `<li>`.