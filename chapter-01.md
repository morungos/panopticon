---
title: Chapter 1 - A Postmodern Panopticon
---
<nav aria-label="Breadcrumb" class="breadcrumb">
  <ul>
    <li><a href='{{ "/" | relative_url }}'>Home</a></li>
    <li><span aria-current="page">{{ page.title }}</span></li>
  </ul>
</nav>

# {{ page.title }} 

> Current draft: {% include _collection_word_count.md collection="chapter-01" %} words

{% for section in sections %}
{% if section.title != '' %} 
## {{ section.title }}
{% endif %}
{{ section.content}}
{% endfor %}
