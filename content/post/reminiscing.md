---
title: "Reminiscing about my first project"
date: 2020-09-25
tags: ["Roots", "Php", "SQL", "Web development"]
draft: false
---
*Disclaimer: A lot of things I did as a kid were dumb. This article is me just
musing at the decisions I made as a 14 year old.*


The very first project that I would consider a "real project"
I did was a website to manage a database for a hypothetical library. 
I had spent the last few months learning SQL and php
and this was my attempt at putting together that knowledge. 
So I designed a SQL database. Wrote some static HTML pages 
where I obviously used tables with no borders as my layout tool. Finally I wrote
some php to generate generate tables in views and read values from some forms in
add and update pages. 

I was extremely proud of what I had built. It was a fully working system
that could manage a log of all the actions in the library, any late fees 
owed by any borrower and had a clear dashboard where most common actions were
aggregated. Honestly, given what my 14 year old self knew about programming,
this was a huge accomplishment. I had proven to myself that everything that I had
learned could be used in a meaningful way. Not only that I had spent a summer
break building something rather than playing video games all day.

### Security?
To be honest I asked my school, which was using a completely
manual process at the time, to use my system and they decided 
against using my project. I couldnt understand it at the time, 
and boy am I glad they chose to not use it. Looking back at the 
code was completely full of security vulnerability. I think I knew
what a SQL Injection was, but I never fixed it. Every text box on 
my website was a security issue. Searching for a book literally 
translated to a SQL string (with a stringf) and was called on the 
database. There was no cleansing of user input and there was certainly
clever use of an ORM that could have potentially saved me from the
problem.


### Source
I did put my code up on github for posterity. Warning: not for the faint of
heart. contains a lot of bad practices

https://github.com/SamedhG/LibManager
I'll try to run the site and put some pictures up in an update.
