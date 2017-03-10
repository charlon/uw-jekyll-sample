---
title: Fruit is cool
layout: small-hero
permalink: /fruit/
---

<h2>{{page.title}}</h2>

Look at this thing he did! Just look at it. asdlkfj

{% for fruit in site.fruit %}
  <div class="cookie">
    <h2><a href="{{ fruit.url }}">{{ fruit.title }}</a></h2>
    {{ fruit.content }}
  </div>
{% endfor %}
