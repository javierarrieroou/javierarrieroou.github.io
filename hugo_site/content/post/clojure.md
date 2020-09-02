+++
author = "Javier Arriero"
title = "Clojure"
date = "2019-03-11"
description = "Clojure development"
tags = [
    "clojure",
    "development",
    "services",
]
categories = [
    "development",
    "services",
]
series = ["Development Guide"]
aliases = ["clojure"]
+++

Clojure is a dynamic, general-purpose programming language, combining the approachability and interactive development of a scripting language with an efficient and robust infrastructure for multithreaded programming. Clojure is a compiled language, yet remains completely dynamic – every feature supported by Clojure is supported at runtime. Clojure provides easy access to the Java frameworks, with optional type hints and type inference, to ensure that calls to Java can avoid reflection.

Clojure is a dialect of Lisp, and shares with Lisp the code-as-data philosophy and a powerful macro system. Clojure is predominantly a functional programming language, and features a rich set of immutable, persistent data structures. When mutable state is needed, Clojure offers a software transactional memory system and reactive Agent system that ensure clean, correct, multithreaded designs.

<!--more-->

## What

1.  Homoiconicity
    Clojure is related to the prominent and elegant Lisp family. One of its main properties is homoiconicity, which causes lively debate among software developers worldwide.

    A language is homoiconic if a program written in it can be manipulated as data using the language. Thus the program’s internal representation can be inferred just by reading the program itself.
    Imagine a Lisp program, which is presented as a normal Lisp list. Meanwhile, you can manipulate it using other Lisp code. So, Clojure developers can access and transform code into data. This Lisp peculiarity shows the concept of “code as data.”

    This feature is conceptually possible because of the minimalist and utterly consistent Clojure syntax. The whole program code is represented via S-expressions (tree-like structures). This is the of same type of code representatoin as that supported by Clojure Core. So, code can be easily transformed into data through macros.

    The strong macro system gives an opportunity to create code that generates other code. It enables software developers to write extensions without waiting for the programming language designers to implement it. The latter is also relevant for writing you own Domain-Specific Languages (DSLs) with the help of macros. They are responsible for the “translation” from your language to Clojure.

    The benefits of well-designed DSLs are obvious. Clojure’s macro system gives you excellent opportunities for using them.

    Writing the internal DSL with these macros leads to a new level of code refactoring. It also expands the language itself with modern elements. They are useful for the implementation of business goals in the context of each specific project.

    The core.async macro in Clojure is one of the best examples of this principle benefit. core.async brings the power of CSP-style concurrency to Clojure. Thanks to the macro, it was created as a library without interrupting the Clojure language.

    Compojure is another popular Clojure library that is based on the homoiconicity principle. 

2.  Functional Approach
    What causes complexity and problems in computer programs? Side effects are among the main factors of our challenges. You can’t fully avoid them. But you can localize the spillovers and the programming language should help you.

    As a functional language, Clojure encourages you to write pure functions. The results of such functions depend only on the input parameters. So, it doesn’t matter how many times you start the function. The result is always the same. This simplifies testing because you don’t have to try various queues and find the right state of inputs.

    Pure functions are also handy for analyzing and refactoring. They are extremely simple, even if they do a great job.

    Clojure's beauty lies in how the language perfectly joins individual elements into a coherent whole.

    Clojure, like JavaScript, operates using functions as values. So, they can be transmitted as parameters and returned from other functions. This provides flexibility for a developer because he/she can delay or customize an on-the-fly logic realization. Moreover, the functional approach enables making the processors middleware by default. So, you can customize them for different business goals, which range from logging to conditional email sending.

3.  Immutable Data Structures
    Clojure has features of an object-oriented language. So, it initially includes a set of immutable (unchangeable) structures and methods for working with them.

    They look like common JavaScript arrays and Hash Maps. But any operation can’t change their values. Instead of changing, it creates an absolutely new structure with updated data.

    The immutability is handy when writing multithreaded applications because it negates a whole class of bugs related to synchronization of changing variables between threads. So, you can build entire information models using the few immutable data structures included in Clojure. The predictable code is easier to write and easier to test, which helps to develop a product quickly.

    For example, look at the FreshCode use case. The development of e-commerce platform that supports more than one million users took just 4 months. It proves that Clojure allows programmers to focus on engineering efforts instead of extra details.

4.  A Multipurpose Solution
    Clojure is a good choice for a wide variety of projects. You can use it from social networking industry to Big Data solutions. Initially, Clojure language was targeted for working with JVM. So, the most popular modern Clojure implementation uses the Java Virtual Machine. This enables simple interaction with Java libraries, creation of Java objects and using the Maven repository. Java platform’s maturity and the huge ecosystem provide many benefits for Clojure developers.

    An interesting fact is that although JVM primarily runs Java, about 3% of JVM users are programming in Clojure. It’s a remarkable fact, which shows the great potential of functional programming and Clojure itself.