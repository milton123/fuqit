The FuqIt Web Framework
=======================

I'm kind of tired of following the stupid rules of MVC and want to just
try out making something where I shit files into a directory and they
just work.  This Python web framework (if you can call it that) is my
first crack at something like that.  I basically did this on a Saturday
morning because I was bored.  If you don't like it, then oh well, life
goes on.

How It Works
============

1. mkdir app
2. touch app/__init__.py
3. python fuqit.py app 0.0.0.0 8080
4. Put .py files or "anything else" into app.
5. The .py files need a run function.  It gets variables.
6. Anything else is a jinja2 template.

That's it.  Look in this project's app/ directory to see me
doing stupid crap with it to see if it works.

Resolution Order
================

Easy, and oh so hackable so don't run this crap on any computer you
care about.

1. If it has an extension it's a template.
2. If it ends in / it's either /index.html or /index.py
3. Otherwise it's a module named after the path with / changed to .

Examples:

* / -> /index.html or /index.py
* /the/stupid/place/stuff.txt -> jinja template same path
* /the/other/place/index.html -> same thing
* /mystuff/cool -> a module named app.mystuff.cool

And if people go to a directory without the slash then that's just tough.
I haven't implemented dumbfuck-do-what-i-mean-redirects yet.

It also can't handle binary files yet.  What a travesty.  I'll do that tomorrow
when I'm bored again.

But That's Magic!
=================

I will refer you to our official Mascot:

![Magic Is Awesome](https://github.com/zedshaw/fuqit/blob/master/mascot.gif?raw=true)

Investor Statement
==================

Do you have a load of money and are you looking for the next Meteor to waste it
on?  Well this project is currently looking for funding and it's already been
on the top of HackerNews!

![HN Too Easy](https://github.com/zedshaw/fuqit/blob/master/hn_win.png?raw=true)

Act fast because pretty soon I'll have a spare Sunday and FuqIt will become
more secure than both Meteor and Ruby On Rails and then you'll miss out on
investing in the next hottest thing.  You'll have to go buy some Gucci hand
bags or a DVF dress to be in-fashion instead.  Can't have that now.


