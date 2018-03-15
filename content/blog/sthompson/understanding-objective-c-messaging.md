---
title: "Understanding Objective-C : Messaging"
description: "<p>In this installment, I hope now to point out some of the unique features of the Objective-C language and entice other"
date: "2011-05-23"
author: "sthompson"
tags:
    - "blog"
---

<p>In this installment, I hope now to point out some of the unique features of the Objective-C language and entice other geeks to look at the language with new eyes. In this case we are going to examine the technique used to invoke object behaviors, message passing.<a href="http://en.wikipedia.org/wiki/Objective-C">Objective-C</a> is the lingua franca of <a href="http://en.wikipedia.org/wiki/Mac_OS_X">Mac OS X</a> and <a href="http://en.wikipedia.org/wiki/Iphone_os">iOS</a> application development. However, the language is seldom seen outside of the Apple development environment. As a result, relatively few developers are exposed to the language. Regular readers of this blog will know that I'm a bit of a language geek. I enjoy learning about different programming languages, their unique structures and the tools they provide to help programmers solve problems. In the coming weeks, I hope to point out some of the unique features of the Objective-C language and entice other geeks to look at the language. In this case we are going to examine the technique used to invoke object behaviors, <a href="http://en.wikipedia.org/wiki/Message_passing">message passing</a>. But first, a historical diversion.</p>
<p>Objective-C was developed in the early 1980s. Like its contemporary, C++, the language evolved as a means of incorporating <a href="http://en.wikipedia.org/wiki/Smalltalk">Smalltalk</a>-like concepts of <a href="http://en.wikipedia.org/wiki/Object-oriented_programming">Object-Oriented programming</a> into the C programming language. This language was eventually adopted as a primary tool for the <a href="http://en.wikipedia.org/wiki/NeXT_Computer">NeXT computer</a> company. Apple acquired NeXT, and the legacy of both Objective-C and the frameworks that were built with it. Those frameworks are the progenitors of today's <a href="http://developer.apple.com/technologies/mac/cocoa.html">Cocoa</a> application environment on Mac OS X, and the UIKit application environment on iOS.</p>
<p>The first thing to know about Objective-C is that it is a strict superset of <a href="http://en.wikipedia.org/wiki/C_(programming_language)">C</a>. That means that an Objective-C compiler should accept a C language program and produce correct output. Exactly what dialect of C a particular compiler will accept is largely vendor specific, but the important point is that if you know how to write C then you already know a significant amount about the Objective-C language.</p>
<p>To this base language, Objective-C adds a number of object-oriented features and includes syntax elements in support of those features. In syntax and semantics those object-oriented features resemble Smalltalk. The Objective-C message passing mechanism plays a central role in these additions. </p>
<p>Because of its roots in Smalltalk, the syntax of Objective-C message passing seems very strange to developers of other languages. However, the sense of oddity fades quickly when working in the language. As an example of this syntax, to ask the file object represented by the <tt>documentFile</tt> variable to set its read position 1024 bytes into the file the message might look something like this:</p>
<pre lang="objc">
[documentFile seekPosition: 1024 relativeTo: FILE_START];
</pre><p>
The square brackets introduce the fact that this statement is passing a message to a file. The first identifier after the opening bracket is the object to which the message is being passed. The rest of the line identifies the parameters of the message and deserves some further explanation.</p>
<p>A good question to ask as this point is: "Exactly what message is being sent to the <tt>documentFile</tt> object?".</p>
<p>In this case the message being passed to the object can be represented as a string: <tt>"seekPosition:relativeTo:"</tt>. This string is known as a Selector. The colons are part of the selector name and string is a whole unit; it cannot be broken into parts. You might imagine another message whose selector is <tt>"seekPosition:"</tt>. In spite of the fact that one selector is a substring of the other, the compiler sees each as a distinct selectors and does <strong>not</strong> recognize the messages as being related in any way.</p>
<p>Be careful as well that you do not perceive this as routine call with labelled parameters. In some other languages this particular method invocation might resemble a single call with two labelled parameters, <tt>seekPosition</tt> and <tt>relativeTo</tt>. That is <strong>not</strong> the case here. Objective-C does not have the concept of labelled parameters. In sending this message there is only one selector in play, <tt>seekPosition:relativeTo:</tt>. The colons indicate that the method invoked by that selector takes two parameters, but the positions of those parameters in the method call are fixed.</p>
<p>The means of making the call, interspersing parts of the selector between the parameters, is another aspect of Objective-C that programmers from other languages must adjust to as the learn the new language. While it is true that it makes Objective-C more verbose than other languages, it also makes it the code very readable as, when <a href="http://developer.apple.com/library/mac/#documentation/Cocoa/Conceptual/CodingGuidelines/CodingGuidelines.html">proper coding conventions</a> are followed, a method call looks very much like an imperative statement "Hey Mr. <tt>documentFile</tt>, seek position 1024 relative to the start of the file!"</p>
<p>Semantically speaking, the behavior of this message passing is a bit different in Objective-C than in other languages like C++, Java, or C#. Objective-C is a <a href="http://en.wikipedia.org/wiki/Dynamic_dispatch">dynamically-dispatched</a> language. That means that the system determines, at run-time, while a program is executing, whether or not a given object responds to a particular message and if so, which method is executed. This is in contrast to C++ which is a statically dispatched language. It is called statically dispatched because the method that a particular call will invoke is determined by the compiler when the code is built.</p>
<p>In Objective-C, a program can send a message to the <tt>documentFile</tt> object that files generally don't understand:</p>
<pre lang='objc'>
[documentFile standUpAndClap]
</pre><p>
The Objective-C compiler will flag a warning on this line indicating that the code is sending a message to the <tt>documentFile</tt> object that it might not understand, however this would not prevent the code from successfully compiling. When this line of code is executed, the system will try to send the <tt>standUpAndClap</tt> message to <tt>documentFile</tt>. If the object does not respond to that selector, if it does not have a method corresponding to that message, then the system will generate a runtime exception.</p>
<p>The power of this system becomes more evident, when you consider that the dynamic nature of Objective-C. The language allows you to add methods to a object (or even more specifically to an object's class) at run time. When the application starts, some agent within the running program could add a method implementation for <tt>standUpAndClap</tt> to the class of the <tt>documentFile</tt> object. Even though that class didn't have an implementation for the method when it was compiled, the object responds to the message at runtime and the application will continue without an exception being thrown. This is a very powerful feature of the language and its run-time system. It allows for sophisticated use of Objective-C. For example, it enables language bridges to other programming systems like <a href="http://en.wikipedia.org/wiki/RubyCocoa">Ruby</a> and Python. It also allows for powerful object serialization tools like Apple's <a href="http://developer.apple.com/library/mac/#documentation/Cocoa/Conceptual/CoreData/cdProgrammingGuide.html">Core Data framework</a>.</p>
<p>The paradigm that uses message passing to invoke object behavior, while not unique to Objective-C, is central to the language and distinguishes it from similar languages such as Java, C++, and C#. Many find the syntax, inspired by Smalltalk, to be unusual at first, but quickly adapt to it as they work with the language. The message passing system is straightforward for basic programming tasks, but rich enough to offer powerful features to more sophisticated applications.</p>
<p>In another installment we will look at the Objective-C class system and inheritance model to see how selectors are used to implement methods and how message passing works with polymorphism and inheritance.</p>
<p>If you are impatient and would like to learn more about Objective-C today, please visit the following resources at Apple's web site and out in the wider internet:</p>
<p><a href="http://developer.apple.com/library/mac/#referencelibrary/GettingStarted/Learning_Objective-C_A_Primer/_index.html">Learning Objective-C: A primer</a></p>
<p><a href="http://developer.apple.com/library/mac/#documentation/Cocoa/Conceptual/ObjectiveC/Introduction/introObjectiveC.html">The Objective-C Programming Language</a></p>
<p><a href="http://developer.apple.com/library/mac/#documentation/Cocoa/Conceptual/OOP_ObjC/Introduction/Introduction.html">Object-Oriented Programming with Objective-C</a></p>
<p><a href="http://www.amazon.com/Programming-Objective-C-2-0-Stephen-Kochan/dp/0321566157">Programming Objective-C (at Amazon.com)</a></p>
<p>In addition many on-line resources exist and are available with a simple search in your favorite search engine.</p>
