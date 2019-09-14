---
---
{% include navigation.html %}

## Home

Welcome to my hub. You can find more information about me or this website [here.](/about.html)

To find a list of my github projects [click here.](/projects.html)

Otherwise I do run an occasional blog for you to enjoy.

## Blog

{% capture nav %}
{% include navigation.html %}
{% endcapture %}
{% assign nav=nav | strip_html | strip_newlines %}

{% assign postsByYearMonth = site.posts | group_by_exp:"post", "post.date | date: '%B %Y'"  %}
{% for yearMonth in postsByYearMonth %}

### {{ yearMonth.name }}

    {% for post in yearMonth.items %}

* [{{ post.title }}]({{ post.url }}) [{{ post.date | date: "%B %-d" }}] "{{ post.excerpt | strip_html | strip_newlines | remove: nav }}"

    {% endfor %}
{% endfor %}
