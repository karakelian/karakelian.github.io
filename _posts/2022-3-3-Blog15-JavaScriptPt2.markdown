---
layout: post
title:  "Blog 15 - JavaScript pt.2"
date:   2022-3-3 5:15:29 -0700
categories: Tech
---
## JavaScript: Going In-Depth
In last weeks blog, we introduced the topic of JavaScript and briefly spoke about its history, client-side usage and features. In this weeks blog, we will be touching upon JavaScript's more advanced topics, including real-world examples of code and implementation with the programming language. As noted before, most major web browsers include the JavaScript engine for code execution on devices for users around the world. Although this puts emphasis on the programming languages flexibility and simplicity for developers, there is more stress on security because of its wide-usage across the web. To cover more advanced topics in this blog regarding JavaScript, we will introduce more features that offer an in-depth look at the programming language, while examining its syntax and security within its implementation. 
<br/><br/>
<img src="https://static.skillshare.com/uploads/discussion/tmp/bfdac8f1" alt="MSC" width="350" height="200">
<br/>

## Advanced Features In JavaScript
Last time we glanced over JavaScript features such as imperative and structure programming, weakly typed coding and dynamic languages. To start off with some in-depth topics, lets cover JavaScripts Object-Orientation model. In this programming language, object-orientation is prototype based and an object is viewed as an associative array. In order to specify a name, the dot notation of `(obj.x=10)` and `(obj['x']=10)` is used, along with properties that allow the developer to add, delete or rebound at runtime. Prototypes in JavaScript also employ classes for inheritance, and functions are used as object constructors. Functional's in JavasScript also include a function to be an object, where properties and methods are part of a function. Some examples of these Functional units are `.call()` and `.bind()`, which can also be nested functions and defined within each other. 
<br/><br/>
That support of Delegatives is also an advanced topic in JavaScript which essentially allows objects to be evaluated as members of another original object. This is also a common element of object-oriented programming. Traits and Mixins are natively supported in this programming language, and this includes roles to be explicitly delegated, such as `apply` or `call`. Other miscellaneous advanced topics include JavaScripts run-time environment, which it relies on to support methods and objects for script interaction. Variadic functions and regular expressions are also supported by JavaScript, and vendir-specific extensions can be added on the JavaScript Engine. Some of these extensions include but are not limited to:
- `Array Comprehensions`
- `Concise Function Expressions, e.g. (function(args) expr)`
- `ECMAScript for XML`
- `Conditional Catch Clauses`
- `Generator Expressions`

## Syntax
Syntax in JavaScript is significant as variables can be defined with keywords such as `let`, `var`, and `const`. These keywords each serve a purpose in declaring function-scoped variables, constant variables, and assignment of literal values. Recursive functions can be employed in JavaScript using the `function` keyword to set function and create `if statements` and `for loops` within. The following code represents a simple recursive function in JavaScript that also utilizes Tail Call Optimizations:
<br/><br/>
<img src="https://miro.medium.com/max/506/1*Lh44XkK8lxwK201Q3SJDTQ.png" alt="MSC" width="350" height="200">
<br/>
Anonymous functions can also be created using counters, where the `let` command can be set to return values in order as they are processed in the function. 
<br/><br/>
<img src="https://miro.medium.com/max/1039/1*ERA5Hj34lNGmNZX63TnyAQ.png" alt="MSC" width="350" height="200">
<br/>

## Security In JavaScript and Disadvantages
Security in JavaScript can have a whole blog dedicated to itself because of the vast features it has acquired over the years. Cross-site vulnerabilities have been an important stepping stone, as cross-site scripting has become a common security problem in JavaScript. They can occur when attackers target websites such as Banks, and include malicious files and scripts to present the user through a webpage. Modern day browsers include partial protection against this but can still be vulnerable to XSS attacks. Cross-site forgery is also a common issue in which attackers trick the browser to take unintended actions. For this reason, browsers require authentication. 
<br/><br/>
Sandbox Implementation errors and browser plugin coding have also been vulnerability issues present to JavaScript, and developers and security programmers alike strive to ensure JavaScript's security by undertaking these issues and their causes. Hardware vulnerabilities are also not uncommon, and just in the past few years have been developments in the `rowhammer attack` and `ASLR Bypass`. These attacks were demonstrated in using JavaScript, and were mostly JavaScript-based in their implementation. More strict security is now the primary focus of JavaScript patches to dissuade hackers from taking advantage of features within JavaScript to produce new vulnerabilities. 

### Learn More About JavaScript
We have covered a lot regarding JavaScript in these past two blogs, but if you are still interested to learn more, visit [JavaScript][web-io] to stay in touch with the latest updates. [W3Schools][learn-io] also offers in-depth tutorials on JavaScript if you wish to get started programming with the language. 
<br/><br/>
Stay tuned for a new blog post next week!

[web-io]: https://www.javascript.com/ 
[learn-io]: https://www.w3schools.com/js/ 
