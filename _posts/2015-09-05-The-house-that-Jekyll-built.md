---
layout: post
title: The house that Jekyll built - understanding the components of the popular static site generator
tags: [Jekyll, Poole, Liquid, Markdown, Sass, Pygments]
description: Understanding how Poole, Liquid, Markdown, Sass, and Pygments work with Jekyll
---

> "May the walls of your blog be sturdy yet pretty, and the roof never collapse upon your head" - *Old proverb*

Introduction
------------

There are many ways to make a blog. If [Wordpress](https://wordpress.com) lies at one end of the spectrum, and starting with a couple of blank HTML and CSS files lies at the other, then I was looking for something in between. A fun way to teach myself web development and use a bunch of cool tools, without the trauma of starting from scratch. I ended up going with [Jekyll](http://jekyllrb.com/) to make my blog, and this was the end result.

One drawback of getting started with Jekyll is that it can be hard to understand from the documentation what the other tools that slot into it (e.g. Liquid, Markdown, Sass) actually do. Phrases like "templating engine", "markup language", and "CSS extension language" don't mean much if you're new to web development.

In this post I'm therefore going to give an overview of what Jekyll is and how these other tools fit in. To help illustrate some ideas I'm going to use a simple analogy - **creating a blog is like building a house**. I'll assume that you're already familiar with the basics of HTML and CSS and are looking to build on that. Remember, key point: **blog = house**.

You
---

To build a house, we need a builder. In our case the builder works on everything - the walls, the rooms, the furniture, the interior design. **You are the builder**. You start off buying a plot of land somewhere *(read: web address and hosting)*.

Jekyll
-----

Building a house is hard work. To help you in your endeavour, **you decide to hire a project manager called [Jekyll](http://jekyllrb.com/)**. The deal is that you will build all the parts of the house yourself, which is good because you're OCD like that, but Jekyll will put them together. So to use the kitchen as an example, you make the layout (e.g. door here, windows there), the furniture/appliances (e.g. counters, fridge, oven), and the decorations (e.g. curtains, paint), then Jekyll fits them together for you.

Poole
------

Building a house is unfortunately still hard work, even with the help of a project manager. You begin to look around the neighbourhood for ideas about features (e.g. garden, garage) and design (e.g. colours, shapes). Just when you tear down the kitchen for the 5th time and are ready to go back to renting, Jekyll says - "what if I gave you a free, unfurnished, extensible 1 bedroom house to put on your plot of land? I built it during my last project. It's not the end product, we still need to add 2 more rooms and redecorate the hallway, but it's a flying start". You gratefully accept and the next day your **1 bed house called [Poole](https://github.com/poole/poole)** arrives.

Liquid
------

Your house is now starting to take shape. You thank Jekyll for all the help, until he/she tells you a secret. "*[Your name]*, I hate to tell you this but I actually have a friend helping me downstairs. **[Liquid](http://liquidmarkup.org/) is a technician and automates some things for us**. For example, all rooms have certain features, like a ceiling and a floor *(read: a header and a footer)*, and Liquid has been fitting these automatically". After pondering on this news for a while, you decide you are glad to have Liquid around since he/she stops you from having to repeat yourself. Liquid is quite particular about your instructions, but you don't interact with him/her very much after the first few days.

Markdown
--------

You have a big family, and might end up with a lot of bedrooms *(read: blog posts)* in your house. It takes you a long time to build each bedroom yourself so you say to Jekyll - "Jekyll my man/woman, meet [Markdown](https://daringfireball.net/projects/markdown/)". **Markdown is a workman who enables you to build bedrooms more quickly**. For instance, you give Markdown a block of wood *(read: plain text)* and put a sticker on it saying "bed", then Markdown creates a bed *(read: HTML)* for you.

Sass
----

Markdown is doing a great job but he/she is rubbish when it comes to design. I'd be embarrassed to sleep in that bed. So you hire another person, **[Sass](http://sass-lang.com/), an interior designer**. Sass won't actually do the design, that's your job, but he/she improves upon the usual *(read: CSS)* method that you use. For example you might say to yourself "a dining room is really just a subset of a living room, so we'll use the same table design in both". Sass will help you do this efficiently.

Pygments
--------

Our house is now built and there is only one other person standing around who you've been afraid to talk to. You finally ask them what the hell they've been doing in the garden all this time. "Oh I'm **[Pygments](http://pygments.org/), the photocopy guy**" they say. "I'm just here in case you want to easily share a copy of the design of your house *(read: code)* with your friends and make it look nice". You breathe a sigh of relief - Pygments is not critical to the construction of your house. You make a mental note to call him/her at a later date should you decide to share any designs.

Conclusion
----------

So there you have it. Hopefully you now understand how all the components of Jekyll fit together a bit better and are eager to start building a house of your own. 

Of course Markdown, Sass etc can all be swapped for other assistants who have different names but do a similar thing - I just used the built-in ones as an example. Some people avoid using them altogether; it's up to you. I've also had to simplify many things, such as the rules that Jekyll follows to fit your house and how Liquid uses templates to automate things.

What did you think of my little analogy? Was it useful? Comments are 'on the house'.

*p.s. If you're looking for a walkthrough of getting a site set up using Jekyll, I can recommend [this excellent post from Joshua Lande](https://joshualande.com/jekyll-github-pages-poole/). I also borrowed a few nice ideas from [Alex Pearce](https://alexpearce.me/2012/04/simple-jekyll-searching/).*
