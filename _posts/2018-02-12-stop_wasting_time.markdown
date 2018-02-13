---
layout: post
title:      " "stop wasting time""
date:       2018-02-13 03:20:29 +0000
permalink:  stop_wasting_time
---


it was the 70 to 80th commit of the Rails Project, which I had endeavored to replicate a Zoho Creator application I started in 2012, and to CRUD through one Domain and its nested attributes. 

Replicating the application

The application Zoho Creator Domains for an Order has deadlines, frequency of the deadline, sites, tasks(1 thru 30 or more), datetime pickbox, and comment for each order. I attempted, but after 2 weeks, it became evident that one level deep nested level prevents me from creating separate domains(class) for each feature.  

After accounting for the time(14 hours) and success/failure rate: 44% success rate of 60 different ideas, I rested with the only reasonable options: place feature options as an attribute of the Order object form.   Instead, according to Rails Doc, I should just place the feature options as an attribute of the Order object form. 

CRUD through one domain and its nested attribute

With accounting came change, I was stuck at Updating portion of the CRUD. I read and read and read until I came across Ryan Bates Rails Cast on Virtuous Attributes and nested forms. Ryan mentioned how to use attr_accessor and attr writer to update a field in an object, while the field_for (comments in my case) is in a many-to-many relationship to the form for object(Order in my case).  Ryan also mentioned that the Rails doc regarding nested attributes were lacking
               '....but it less clear on how we would get this working in the view itself, so we’ll focus on this.'

Now unto other objectives in life.







