---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

{% if site.author.googlescholar %}
  <div class="wordwrap">You can also find my articles on <a href="{{site.author.googlescholar}}">my Google Scholar profile</a>.</div>
{% endif %}

{% include base_path %}

<div style="padding-top: 50px;">
## Publication
{% for post in site.publications reversed %}
  {% if post.pubtype == 'publication' %}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}
</div>
<div style="padding-top: 50px;">
## Working Paper
{% for post in site.publications reversed %}
  {% if post.pubtype == 'workingpaper' %}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}
</div>
<div style="padding-top: 50px;">
## Work in Progress
{% for post in site.publications reversed %}
  {% if post.pubtype == 'workinprogress' %}
      {% include archive-single.html %}
  {% endif %}
{% endfor %}
