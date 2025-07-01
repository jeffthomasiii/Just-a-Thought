---
layout: page
title: Tags
permalink: /tags/
---

# 🏷️ Tags

Here’s a breakdown of topics I’ve been reflecting on. Click a tag to jump to related posts.

## 📚 Tag Index

<ul>
  {% assign tags_list = site.tags | sort %}
  {% for tag in tags_list %}
    <li><a href="#{{ tag[0] | slugify }}">{{ tag[0] }}</a> ({{ tag[1].size }})</li>
  {% endfor %}
</ul>

---

## 🔖 Posts by Tag

{% for tag in tags_list %}
### <a id="{{ tag[0] | slugify }}"></a>{{ tag[0] }}

<ul>
  {% for post in tag[1] %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      <br><small>{{ post.date | date: "%B %-d, %Y" }}</small>
    </li>
  {% endfor %}
</ul>
{% endfor %}
