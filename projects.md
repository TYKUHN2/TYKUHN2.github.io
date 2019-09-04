---
title: Github Projects
---
{% include navigation.html %}

Here you can find a variety of my projects, generally active ones, in a variety of languages for a variety of purposes. Variety!

## Github Projects

{% for project in site.data.github %}

* [{{ project.name }}](https://github.com{{ project.link }}) - {{ project.short_desc }}
{% endfor %}
