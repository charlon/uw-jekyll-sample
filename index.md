---
layout: big-hero
title: home
---

<div class="home">

    <p>welcome to jekyll!</p>

    <ul class="post-list">
        {% for post in site.posts %}
        <li>
            <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }} - {% for category in post.categories %}{{category}}, {% endfor %}</span>
            <h2><a class="post-link" href="{{ post.url | relative_url }}">{{ post.title | escape }}</a></h2>
        </li>
        {% endfor %}
    </ul>

</div>
