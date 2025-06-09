---
title: Home Page Content 
---
<div>
{% for post in site.posts %}
        <a href="{{ site.baseurl }}{{ post.url }}">
                <!-- Post Image -->
                {% if post.image %}
                <img src="{{ post.image | relative_url }}" alt="{{ post.title }}">
                {% else %}
                <!-- Placeholder image if no image is defined in the post's front matter -->
                <img src="{{ /assets/images/placeholder.jpg | absolute_url }}" alt="Placeholder image for {{ post.title }}">
                {% endif %}
            </a>
        <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
            <p>
                {{ post.excerpt }}
            </p>
{% endfor %}  
</div>