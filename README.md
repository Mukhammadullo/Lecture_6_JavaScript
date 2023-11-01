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
console.log(forTxt); //Output:


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
