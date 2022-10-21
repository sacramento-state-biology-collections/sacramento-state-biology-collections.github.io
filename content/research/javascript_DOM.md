---
title: "Editing the HTML Document Object Model with Javascript"
date: 2022-10-14T15:45:20-07:00
draft: false
---

## What is the HTML Document Object Model?

<center><img src="/img/JavascriptDomExamples/DOM_example.jpg"></center>

---

The HTML Document Object Model (DOM) is a standard object model and programming interface for HTML. It is the standard for how to get, change, add, or delete HTML elements. 

## How to Interact with the Content of an HTML Page

Each HTML element can have a name, label, or id. Javascript can use these to interact with the element.
Example: <center><img src="/img/JavascriptDomExamples/e1.jpg"></center>

The textarea has the id 'text' for javascript to use. It does this by using 

``` PowerShell
document.getElementByID("text");
```
You can read the user's input in that textarea by using

``` Powershell
let str = document.getElementByID("text").value;
```
You can now do whatever you want to that string.

## Further Reading

[JavaScript DOM Detailed Info](https://www.w3schools.com/js/js_htmldom.asp)