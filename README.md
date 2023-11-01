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

