# XML and DOM API

The example demonstrates the use of CSS for styling XML data and the use of DOM API for accessing the XML DOM.

The DOM defines a standard for accessing and manipulating documents:

>The W3C Document Object Model (DOM) is a platform and language-neutral interface that allows programs and scripts to dynamically access and update the content, structure, and style of a document.

The HTML DOM defines a standard way for accessing and manipulating HTML documents. It presents an HTML document as a tree-structure.

The XML DOM defines a standard way for accessing and manipulating XML documents. It presents an XML document as a tree-structure.

Understanding the DOM is a must for anyone working with HTML or XML.

Here is an example XML data and its representation as a DOM tree:
```xml
<?xml version="1.0" encoding="UTF-8"?>
<bookstore>
  <book category="cooking">
    <title lang="en">Everyday Italian</title>
    <author>Giada De Laurentiis</author>
    <year>2005</year>
    <price>30.00</price>
  </book>

  <book category="children">
    <title lang="en">Harry Potter</title>
    <author>J K. Rowling</author>
    <year>2005</year>
    <price>29.99</price>
  </book>
</bookstore>
```
![dom tree](nodetree.gif)

* apply style/presentation information to XML using CSS.
```xml
<?xml version="1.0" encoding="utf-8"?>
<?xml-stylesheet type="text/css" href="first_xml_file.css"?>
<FirstTag>
  This is our first XML file
  <!-- This is a comment -->
</FirstTag>
```
The browser know how to use the information in the following CSS file to style this XML file.
```css
FirstTag {
  display: block;
  font-family: Arial;
  font-size: large;
  color: blue;
}
```
A more complex example can be found in [cd_catalog.xml](cd_catalog.xml) and [cd_catalog.css](cd_catalog.css).

* use the DOM API to extract information from XML data to build a web page.

  The example code can be found in [book_dom_example.html](book_dom_example.html) and [book_dom_example2.html](book_dom_example2.html).

## Reference
* w3schools XML tutorial https://www.w3schools.com/xml/default.asp
