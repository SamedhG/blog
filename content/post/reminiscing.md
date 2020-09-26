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
It was a basic GUI to manage a relational database. It had forms to add entries
and tables to view the tables and certain common joins. It also had a fairly
useful global search that would search across members and books. The biggest 
gap in quality was my inexperience, the features where there and they worked as
intended but there was a huge lack of polish.

### Architecture and "design"
I had spent the last few months learning SQL and php and this was my attempt at 
putting together that knowledge. 


I designed a relational database schema which had books and members along with a
log table that kept track of borrowing and returns. Some static HTML pages was
all I used, I had never use JavaScript at the time and while every tutorial on
web design would tell me to use JS, I resisted to maintain the scope of te
project. (In hindsight, using some JavaScript would have made things easier).
As with any amateur project,  tables with no borders was my layout tool. Finally,
I wrote some php that managed logging in, session variables and to generate 
and execute SQL queries. which would either printed as tables or insert rows.

Please never do this:
{{< gist SamedhG bb5e54bd308f97dec4448a69d8db396e >}}

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
against using my project. I couldn't understand it at the time, 
and boy am I glad they chose to not use it. Looking back, the 
code was completely full of security vulnerabilities. I think I knew
what a SQL Injection was, but I never fixed it. Every text box on 
my website was a security issue. Searching for a book literally 
translated to a SQL string (with string concatenation) and was called on the 
database. There was no cleansing of user input and there was certainly
clever use of an ORM that could have potentially saved me from the
problem.

### Source
I did put my code up on github for posterity. Warning: not for the faint of
heart.

https://github.com/SamedhG/LibManager
I'll try to run the site and put some pictures up in an update.
