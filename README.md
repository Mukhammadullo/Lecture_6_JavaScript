# _1.What is the DOM in JavaScript?_
> _The Document Object Model (DOM) is a programming interface for web documents. It represents the page so that programs can change the document structure, style, and content. The DOM represents the document as nodes and objects; that way, programming languages can interact with the page._

>_According to the Document Object Model (DOM for short), every HTML tag is an object. Subtags are "children" of the parent element. The text that is inside the tag is also anobject.All these objects are available with JavaScript, we can use them to modify the page._

> * JavaScript can modify all HTML elements on a page-JavaScript может изменять все элементы HTML на странице.
> * JavaScript can change all HTML attributes on a page-JavaScript может изменять все атрибуты HTML на странице.
> * JavaScript can change all CSS styles on a page.-JavaScript может изменить все стили CSS на странице.
> * JavaScript can remove existing HTML elements and attributes.-JavaScript может удалять существующие элементы и атрибуты HTML.
> * JavaScript can add new HTML elements and attributes.-JavaScript может добавлять новые элементы и атрибуты HTML.
> * JavaScript can respond to all existing HTML events on the page.-JavaScript может реагировать на все существующие HTML-события на странице.
> * JavaScript can fire new HTML events on a page.-JavaScript может запускать новые события HTML на странице.

> ### _querySelector-The querySelector() method returns the first child element that matches a specified CSS selector(s) of an element, querySelectorAll() method can be used to access all elements which match with a specified CSS selector._


```js && html

//1-with className
//HTML
<h1 class="txt">Text in HTML</h1>

//JS
let forTxt=document.querySelector(".txt")
console.log(forTxt); //Output: *Element from HTML


//2-with idName
//HTML
<h1 id="txt">Text in HTML</h1>

//JS
let forTxt=document.querySelector("#txt")
console.log(forTxt); //Output:


//3-with selector
//HTML

<h1>Text in HTML</h1>

//JS
let forTxt=document.querySelector("h1")
console.log(forTxt); //Output:
```

> ### _innerHTML-innerHTML is a property in JavaScript that allows you to get or set the HTML content inside an element. It's a convenient way to access or modify the HTML within an element using JavaScript.-InnerHTML — это свойство JavaScript, которое позволяет получать или устанавливать HTML-содержимое внутри элемента. Это удобный способ получить доступ к HTML-коду элемента или изменить его с помощью JavaScript._

```js

//HTML
<h1>Hello in HTML</h1>

//JS
let txt=documnet.querySelector("h1")
txt.innerHTML="Bye"
console.log(txt) //Output:Bye

```

> ### _Styling DOM Element_

```js

//HTML
<h1>Style in HTML</h1>

//JS
let txt=document.querySelector("h1")
txt.style.color="red"

//output: h1->color red
```

> ## _Events in JavaScript-A JavaScript can be executed when an event occurs, like when a user clicks on an HTML element.To execute code when a user clicks on an element, add JavaScript code to an HTML event attribute:_

```js
<!DOCTYPE html>
<html>
<body>

<h2>JavaScript HTML Events</h2>
<h2 onclick="this.innerHTML='Hello!'">Click on this text!</h2>

</body>
</html>
```

## _appendchild() && append-The appendChild() method appends a node (element) as the lastchild of an element.appendChild() adds a node to the end of the list of children of the specified parent node. If the given child element is a reference to an existing node in the document, then the appendChild() function moves it from its current position to the new position_
```js
// HTML: <div id="myDiv" class="foo bar"></div>

const element = document.getElementById('myDiv');

element.classList.add('baz'); // Adds 'baz' class to the element
element.classList.remove('foo'); // Removes 'foo' class from the element
element.classList.toggle('bar'); // Toggles 'bar' class (removes it in this case)
console.log(element.classList.contains('baz')); // Outputs: true
console.log(element.classList.item(0)); // Outputs: 'baz'
console.log(element.classList.length); // Outputs: 2

```

## _ClassListIn JavaScript, the classList is a property of an HTML element that represents a collection of all the classes assigned to that element. It provides methods to manipulate the classes of an element easily. The classList property is an instance of the DOMTokenList interface._
> * add(className): Adds the specified class to the element's class list.
> * remove(className): Removes the specified class from the element's class list.
> * toggle(className): Toggles the presence of the specified class in the element's class list. If the class is present, it is removed; otherwise, it is added.
> * contains(className): Checks if the element's class list contains the specified class and returns a boolean value indicating the result.
> * item(index): Returns the class name at the specified index in the element's class list.
> * length: Returns the number of classes in the element's class list.
```js
// HTML: <div id="myDiv" class="foo bar"></div>

const element = document.getElementById('myDiv');

element.classList.add('baz'); // Adds 'baz' class to the element
element.classList.remove('foo'); // Removes 'foo' class from the element
element.classList.toggle('bar'); // Toggles 'bar' class (removes it in this case)
console.log(element.classList.contains('baz')); // Outputs: true
console.log(element.classList.item(0)); // Outputs: 'baz'
console.log(element.classList.length); // Outputs: 2

```

# _What is BOM?_
> _The Browser Object Model (BOM) There are no official standards for the Browser Object Model (BOM)._
>_The Window Object_
> * The window object is supported by all browsers. It represents the browser's window.
> * All global JavaScript objects, functions, and variables automatically become members of the window object.
> * Global variables are properties of the window object.
> * Global functions are methods of the window object.
> * Even the document object (of the HTML DOM) is a property of the window object: 
