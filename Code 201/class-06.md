# Objects, and the DOM
## Chapter 3 “Object Literals”
## Object & Method
* Object group together a set of variables and functions to create a model of a something you would recognize from the real world. In an object, variables and functions take on new names.
* If a variable is part of an object, it is called a property. Properties te ll us about the object, such as the name of a hotel or the number of rooms it has. Each individual hotel might have a different name and a different number of rooms.
* If a function is part of an object, it is called a method.Methods represent tasks that are associated with the object. For example, you can check how many rooms are available by subtracting the number of booked rooms from the total number of rooms. 
* properties and methods have a name and a value.
* In an object, that name is called a key, each key should be a uniqe and cannot have 2 keys with the same name.

#### **Example with some lines of code**

![object-firstCode](https://github.com/masalha-96/reading-notes/blob/main/pics/201/class-06/object-code.png?raw=true)


<br>
---
---
<br>

## Chapter 5: “Document Object Model (DOM)”
* **The Document Object Model (DOM)** specifies how browsers should create a model of an HTML page and how JavaScript can access and update the contents of a web page while it is in the browser window.

* The DOM specifies the way in which the browser should structure this model using a DOM tree.
* The DOM is called an object model because the model (the DOM tree) is made of objects.
* Each object represents a different part of the page loaded in the browser window.
* **Application Programming Interface (API)**. User interfaces let humans interact with programs; APls let programs (and scripts) talk to each other.

![DOM Tree](https://techbymarty.files.wordpress.com/2015/12/dom-tree.png?w=840)


### Each node is an object with methods and properties.

1. **The Document Node** it represents the entire page.
2. **Element Nodes** HTML elements describe the structure of an HTML page. (The `<h l > - <h6> `elements describe what parts are headings; the `<p>` tags indicate where.
3. **Attribute Nodes** The opening tags of HTML elements can carry attributes and these are represented by attribute nodes in the DOM tree. **Attribute nodes are not children of the element that carries them; they are part of that element**
4. **Text Nodes** Once you have accessed an element node, you can then reach the text within that element. This is stored in its own text node.



### Accessing and updating the DOM tree involves two steps:
1. Locate the node that represents the element you want to work with.
2. Use its text content, child elements, and attributes.



### Working with The DOM Tree

* **STEP 1: Access The Elements**
     * Select an Individual Element Node : 
         1. `getElementByld ('id')` Uses the value of an element's id attribute (which should be unique within the page).
         2. `querySelector('css selector')` Uses a CSS selector, and returns the first matching element.
    * Select Multiple Elements (Nodelists):
         1. `getElementsByClassName('class')` Selects all elements that have a specific value for their class attribute.
         2. `getElementsByTagName('tagName')` Selects all elements that have the specified tag name .
         3. `querySelectorAll('css selector')`Uses a CSS selector to select all  matching elements.
    * Traversing Between Element Nodes :
         1. `parentNode` Selects the parent of the current element node (which will return just one element).
         2. `previousSibl ing / nextSibl ing` Selects the previous or next sibling from the DOM tree.
         3. `firstChild / lastChild` Select the first or last child of the current element.

* **STEP 2: Work With Those Elements**
     * Access/Update Text Nodes :
         * `nodeValue`  This property lets you access or update contents of a text node.
    * Work With Html Content : 
         1. `innerHTML` One property allows access to child elements and text content:
         2. `textContent`  just the text content: .
         3.  `create Element() , createTextNode() ,appendChild () / removeChild ()`Several methods let you create new nodes, add nodes to a tree, and remove nodes from a tree.
    * Access or Update Attribute Values :
         1. `hasAttribute()` checks if an attribute exists.
         2. `getAttribute()` gets its value.
         3. `setAttribute()`updates the value.
         4. `removeAttribute()` removes an attribute.
