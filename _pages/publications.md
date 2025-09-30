---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% for post in site.publications %}
  <h3>{{ post.title }}</h3>
  <p><strong>{{ post.venue }}</strong> | {{ post.date | date: "%B %Y" }}</p>

  {% if post.paperurl %}
    <p><a href="{{ post.paperurl }}" target="_blank">📄 View Paper</a></p>
  {% endif %}

  {% if post.abstract %}
    <details>
      <summary><strong>🔍 View Abstract</strong></summary>
      <p>{{ post.abstract }}</p>
    </details>
  {% endif %}

  {% if post.bibtexurl %}
    <p><a href="{{ post.bibtexurl }}" target="_blank">📚 BibTeX</a></p>
  {% endif %}

  <hr>
{% endfor %}
