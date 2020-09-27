---
title: "Automating Your Homework"
date: 2020-09-27
tags: ["School", "Homework", "Learning", "Automation"]
draft: false
---
Last weekend one of my roommates (who was taking his first class in
propositional logic) asked me about truth tables. He joked about how
tedious and error prone this task is and I should automate the problem.
So, partly as a challenge to myself I decide to do it. About a 100 lines
of rust later I was generating latex truth tables by parsing the equations
from user input. But interestingly thinking back I have been automating homework
for such a long time. In my second semester of university there was a class that
had us write class templates in a specific format. Some Java reflection later we
had a script to generate the template string from the code saving me
that tedium. 

## Should You do it?

Only do it if you do it yourself. 

When someone learns something new essentially their job is that of abstracting
the knowledge. The point of doing several problems in a math assignment is to
give your brain data points to notice patterns in all those problems. Only when
you have truly understood the problem in the abstract can you generalize it to a
automated program. If anything the task of automating the task is one of
learning.

The argument against automating the homework is "doing is learning", but
this is certainly not true for those of us who to chose to automate the work
ourselves. On the other hand, one can find the script that generates the table
on github; while they would have also automated the work, they would have not
understood the abstraction behind the problem. 

With technologies like GPT-3, many tasks that we don't traditionally
consider pattern driven like writing will start becoming automatable. This
would be a useful thing to do if you noticed the abstractions in the structure
of the writing and can derive the conclusions needed to make that automation do
your bidding for you. If anything with this process you would have learned more 
about writing than you would have if you wrote the paper yourself.

Automating a task will always be harder than the task itself because you can
stumble to the solution when doing the task but you need to truly understand the
problem if you want to automate the solution. 

So automate your homework and be proud of it!


## Source

Heres the code for the truth table generator I wrote:
https://github.com/SamedhG/truth-table-rs

