---
layout: default
title: Index
---
# {{ page.title }}

> "Any sufficiently advanced technology is indistinguishable from magic."  
> - Arthur C. Clarke

Programming might seem like magic to some people but it is not. Knowing how to teach computers to do what you want them to do is a craft, which can be learned.

# Tutorials
{% for post in site.posts reversed %}
1. [{{ post.title }}]({{ site.baseurl }}{{ post.url }}){% endfor %}

# Examples
[Finished programs from tutorials.]({{ site.github.repository_url }}/tree/master/examples)
