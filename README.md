# HumanScript

_**This is a work in progress**._

**Human Script** is a concept of short, human language like sentences, originally described in English with the possibility of implementation in other human languages which represent a ultimate high level layer or programming language which with subsequently be transpiled to the target programming language which in turn will be compiled or built to machine code or bytecode and ran on the target machine.


The 2 original main purposes of **Human Script** are:
1. To be used by people like a designer who haven't had the opportunity to learn, or are not interested in learning a programming language, but want to be able to program simple tasks, for example, listening to a button click and toggling a text block.
2. People with limited to zero experience in programming, who want to get familiar with fundamental programming concepts like variables, conditions, events, and loops, before diving into more advanced topics or programming.

As an example, the following **Human Script**:

```
Start these wisest. Note: This can be either wisest (on page loaded) or earliest (as soon as the code is loaded).
We have a blue button, a red button and a text block.
Set the blue button, to "blue-button" and the red button, to "red-button".
When the blue button, is clicked do toggle the text block.
When the red button, is clicked do set the document's title, to "New title!".
```

To the following **JavaScript** in a browser environment:

```JavaScript
// This can be either wisest (on page loaded) or earliest (as soon as the code is loaded).
document.addEventListener('DOMContentLoaded', 
function()
{
    var blueButton = "blue-button", redButton = "red-button", textBlock = "text-block";
    document.getElementById(blueButton).addEventListener("click", function(){
        document.getElementById(textBlock).style.display = document.getElementById(textBlock).style.display === "none" ? "" : "none";
    });
    document.getElementById(redButton).addEventListener("click", function(){
        document.title= "New title!";
    });
}
, false);
```
