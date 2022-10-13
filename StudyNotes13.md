# DOCUMENT OBJECT MODEL (DOM)

- Document object model (Dom) is an Application Programming Interface (API) which manipulates HTML documents.
- Document object model represents HTML files documents as a tree of nodes. It provide functions which allows us to add, remove and modify parts of the document effectivelThis is a structured representation of HTML documents. It allows JavaScript to access and manipulate HTML elements and styles. It is automatically created by the browser as soon as the page loads. DOM and its methods are part of Web APIs. Web APIs are libraries that browsers implement which can be accessed by JavaScript code.

## DOM TREE STRUCTURE

![DOM Tree Structure](./Blank%20diagram(3).jpeg)
The above diagram depicts the structure of a DOM tree.
- Whatever elements are present in the HTML document will be present in the DOM tree. Each element in the HTML there is one element node in the DOM tree.
- ```Document``` is a special object that JS has access to, it serves as an entry point to the DOM because it is needed to start selecting elements. It has a number of child elements that correspond with HTML elements.
- First child element of document is the HTML element (```<html>```). It has two child elements, the head (```<head>```)and the body (```<body>```) elements. Inside these there are more child elements and so on and so forth.
- DOM tree has more than just element nodes, it also has nodes for text, comments etc. as shown in the diagram above.

## SELECT ELEMENTS

- There are several methods that can be used to access elements, all you need to know is the name of the class or id of the element being manipulated. The first line of code below shows a way of accessing the contents of an element using the ```querySelectorMethod()``` and CSS selectors and the second line of code shows a way of changing the content of the element selected.
        document.querySelector('.message').textContent;
        document.querySelector('.message').textContent = 'Winter is comming';
- The ```document``` is the object represents your web page. To access any element in an HTML page, you always start with accessing the document object.
- The ```querySelector('.message')``` method returns the first child element that matches a specified CSS selector of an element, ```.className``` for classes and ```#IDName``` for IDs. In this case the element being accessed was assigned a class named ```message```.
- The ```.textContent``` property returns or sets the text content of the specified node and all its descendants.
- When accessing the contents of an input field one has to use the ```.value``` property. This property is used to return or set the value of an input.

