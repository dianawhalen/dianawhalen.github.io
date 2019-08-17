---
layout: post
title:      "Sinatra. The framework, not the singer."
date:       2019-08-17 21:39:56 +0000
permalink:  sinatra_the_framework_not_the_singer
---


This project's requirements were fairly straightforward; create a RESTful CMS, CRUD, MVC app, using Sinatra/ActiveRecord.

Sounds simple enough, right? But... when breaking down all the components necessary to building such an application, things get just a little bit more tangled. Just a little. (Hahaha)

For starters, let's get the alphabet soup sorted out, and maybe it all starts making more sense. 

* **REST**: Representational State Transfer. Software architecture style/standard for web applications. Tl;dr: matching our URLs to HTTP verbs to CRUD actions to Controller Routes to rendered Views.

* **URL**: Uniform Resource Locator. (Web address pointing to the resource you want, ie the content, file, etc...)

* **HTTP**: Hyper Text Transfer Protocol. Basically a standardized way for your browser (client) to communicate with a server, and transfer data back and forth.

* **CMS**: Content Management System. Self-explanatory really.

* **CRUD**: Create, Read, Update, Delete. These actions are enacted upon resources (files) that are persisted to a database.

* **MVC**: Model View Controller. An architectural design pattern for developing applications, which is divided into three interconnected parts. It serves to separate the logic from the interface, and manages the behavior, data, and communication within the application stack.

* **Sinatra**: A lightweight Ruby framework and DSL, for developing web applications.

* **DSL**: Domain Specific Language.

* **ActiveRecord**: A Ruby library and DSL for working with Relational SQL Databases. It provides an ORM, in order to map Ruby objects to a database table, methods mapped to table columns and inferred from the database schema, as well as pre-defined CRUD methods.

* **SQL**: Structured Query Language. A standard language for talking to databases.

* **ORM**: Object Relational Mapping.


As an end user, I'm very familiar with using apps, and how generally consistent that experience is. I am presented with choices: items to click or tap, and fields to populate. Easy peasy. As a developer though, being behind the curtain means having to think about all the actions, connections, and interactions needed to make that happen. It's like being a wizard, only cooler.

What I like most about Sinatra, is that in some ways it's the best of both worlds, those worlds being a programming language like pure Ruby, and a larger framework like Rails. Making this kind of application without leveraging a framework would be more involved, having to declare methods manually and extracting them to a Module for ease of use and avoiding unnecessary repetition. 

On the other hand, a larger framework does a lot for you automagically, which can make it hard to fully grasp what is happening under the hood. For this reason, Sinatra is a good intermediary for both learning purposes, and deploying lightweight applications.

Initially, I approached this project with the intent of making it much more complex, with several more models and types of relationships, but it occured to me that I could easily go down a rabbit hole, finding ever more difficult ways to associate and pivot data, something that would be better suited for a larger project leveraging more powerful tools. I opted for keeping this one on the simpler side, showcasing what Sinatra can do. So I went leaner this round.

I created two models, one for a user, and another for toys, to create simple CMS application to track collectibles and figurines. A user is able to create, retrieve, update, or delete their account (yay CRUD), and able to see the pages and forms that correspond to these actions, which persist to a database.

A user's input is also validated so that invalid data isn't persisted, and is authenticated to the user's unique login. Other users' collections are viewable to all users, but cannot be modified or deleted by anyone other than the user who created the toys in their collection.

The toy model includes a number of attributes that can be filled by the user, such as name, edition, color, designer, and brand. 

While this application itself is quite simple, it was an excellent foray into MVC architecture, ActiveRecord, and frameworks, as  well as a useful exercise in managing and controlling data.












