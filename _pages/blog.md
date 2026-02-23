---
title: "Blog"
layout: archive
permalink: /blog/
entries_layout: grid
show_excerpts: true
classes: wide
author_profile: true
redirect_from:
  - /posts/
---
{% include archive-filters.html %}

{% assign visible_posts = site.posts | where: "blog_visible", true %}

<div class="entries-{{ page.entries_layout | default: 'list' }}">
  {% for post in visible_posts %}
    {% include archive-single.html type=page.entries_layout %}
  {% endfor %}
</div>