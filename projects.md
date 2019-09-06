---
title: Github Projects
---
{% include navigation.html %}

Here you can find a variety of my projects, generally active ones, in a variety of languages for a variety of purposes. Variety!

## Github Projects

{% for project in site.data.github %}

* [{{ project.name }}](<https://github.com{{ project.link }}>) - {{ project.short_desc }}
{% endfor %}

## Additional Projects

Currently I have several private projects intended solely for private use or which are not currently ready for public release. These are typically kept in Git repositories stored in Azure DevOps. As such not all of the projects may be currently or ever publicly announced.

I do accept volunteers to help me with private projects but I may be somewhat more restrictive in who I accept.
