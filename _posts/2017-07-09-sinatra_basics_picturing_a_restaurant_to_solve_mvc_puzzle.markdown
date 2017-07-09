---
layout: post
title:  "Sinatra Basics: Picturing a Restaurant to solve MVC puzzle"
date:   2017-07-09 03:43:23 +0000
---


I have always had a hard time of thinking in words when it comes to concepts.  Avi helped to solve the Model View Controller idea when he mentioned the Restaurant

The model is the Chef.  The View is the User. The Controller is the Waiter.  

The Chef only knows what to make, The Waiter only knows when and why, while The Customer only knows the final product. 

Knowing what to make is the job of the Model through Ruby defined methods.  

Controllers, through HTTP verbs, implements the route received from User through the browser, and implement an instance of the Application Controller when the server is up and running. Controller contains the logic of the application between interface and flow of the application from User Browser and Server. 

The view is displayed in '.erb' files and are named to matched the rendering actions. For instance, a GET request to '/' names a file called 'index.erb'.  There are two types of tags, substitution <%= %>, and scripting tab <% %>.  In substitution tag, ruby codes are evaluated and displayed; however, in scripting tags, ruby codes are evaluated but not displayed.





