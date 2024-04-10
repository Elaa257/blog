---
layout: home
title: "Welcome to my blog!"
---

<br/>
<div class="list-group">
    {% for post in site.posts %}
        <a href="{{ post.url }}" class="list-group-item list-group-item-action">
            <div class="d-flex w-100 justify-content-between">
                <h5 class="mb-1">{{ post.title }}</h5>
                <small class="text-body-secondary">{{ post.date | date: "%b %-d, %Y" }}</small>
            </div>
            <p class="mb-1">{{ post.excerpt }}</p>
            <small class="text-body-secondary">{{ post.author }}</small>
        </a>
  {% endfor %}

</div>