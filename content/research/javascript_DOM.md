---
title: "Editing the HTML DOM with Javascript"
date: 2022-10-14T15:45:20-07:00
draft: false
toc: false
---

## What is the HTML DOM?

<center><img src="/img/JavascriptDomExamples/DOM_example.jpg"></center>

---

The HTML Document Object Model (DOM) is a standard object model and programming interface for HTML. It allows javascript to get, change, add, or delete HTML elements. Since each piece of an HTML document has it's own element, javascript can freely modify whatever it needs to.

## How to Use Javascript to Interact with the Content of an HTML Page

Each HTML element can have a name, label, or id. Javascript can use these to interact with the element.

Example: 
``` HTML
<textarea cols="30" rows="4" id="text"></textarea>
```
The textarea has the id 'text' that javascript can use. It does this by using 

``` PowerShell
document.getElementByID("text");
```
You can read the user's input in the textarea by using

``` Powershell
let str = document.getElementByID("text").value;
```
You can now do whatever you want to that string. When you're ready to return the modified string to the document, you can do

```Powershell
document.getElementByID("text").value = str;
```
You've successfully modified an HTML document! There are many other things you can do with other types of HTML elements. As long as it has an id, you're free to make all the changes you want.

## Further Reading

[JavaScript DOM Detailed Info](https://www.w3schools.com/js/js_htmldom.asp)