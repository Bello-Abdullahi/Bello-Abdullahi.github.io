---
layout: archive
title: ""
permalink: /publications/
author_profile: true
---

{% include base_path %}  

Pre Doc Publications
======

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}

<br>

Book chapters
======

{% for post in site.book reversed %}
  {% include archive-single.html %}
{% endfor %}

<br>
