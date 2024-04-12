---
layout: home
title: "Welcome to my blog!"
---

<br/>
<div class="list-group">
    {% for post in site.posts %}
        <a href="{{ post.url }}" class="list-group-item list-group-item-action blogstyle">
            <div class="d-flex w-100 justify-content-between">
                <h5 class="mb-1">{{ post.title }}</h5>
                <small class="text-body-secondary">{{ post.last_modified_at | date: "%b %-d, %Y" }}</small>
            </div>
&nbsp;
            <p class="mb-1">{{ post.excerpt }}</p>
        </a>
<hr/>

  {% endfor %}

</div>