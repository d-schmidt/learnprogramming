---
layout: default
title: Introduction
---
# {{ page.title }}

Programming might seem like magic to some people but it is not. Knowing how to teach computers to do what you want them to do is a craft, which can be learned.

> Most good programmers do programming not because they expect to get paid or get adulation by the public, but because it is fun to program.  
> - Linus Torvalds

I've learned programming at the age of ten, when my dad gave me a [BASIC](https://en.wikipedia.org/wiki/BASIC) book. That was twenty years ago. I still enjoy it and I would like to share some of that fun. If you are willing to try it, I will show you how to get in.

# About these Tutorials
There are (Wikipedia) links everywhere. Feel free to follow them, whenever you want to know more.  
If you get stuck somewhere look at the examples or ask someone! Like [/r/learnprogramming](https://www.reddit.com/r/learnprogramming/)  
Do you find errors? Open an [issue]({{ site.github.repository_url }}/issues)!

# Tutorials
{% for post in site.posts reversed %}
1. [{{ post.title }}]({{ site.baseurl }}{{ post.url }}){% endfor %}

# Examples
[Finished programs from tutorials.]({{ site.github.repository_url }}/tree/master/examples)
