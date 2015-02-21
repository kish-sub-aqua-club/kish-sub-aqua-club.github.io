---
layout: default
title: Current Season Calendar
---
{% assign events = site.categories.events | sort %}
{% for post in events %}
<div class="row event">
  <div class="col-md-3">
    <h3>{{ post.title }}</h3>
    {{ post.when }}
  </div>
  <div class="col-md-9">
    {{ post.excerpt }}
  </div>
</div>
{% endfor %}

