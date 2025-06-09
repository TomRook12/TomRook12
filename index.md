---
title: Home Page Content 
---

<div>
{% for post in site.posts %}
        <a href="{{ site.baseurl }}{{ post.url }}">
                <img src="{{ post.image | relative_url }}" alt="{{ post.title }}">
            </a>
        <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
            <p>
                {{ post.excerpt }}
            </p>
{% endfor %}  
</div>

