---
title: Home Page Content 
---
<div>
{% for post in site.posts %}  
        <a href="{{ site.baseurl }}{{ post.url }}" class="block">
                <!-- Post Image -->
                {% if post.image %}
                <img src="{{ post.image | relative_url }}" alt="{{ post.title }}" class="w-full h-48 object-cover">
                {% else %}
                <!-- Placeholder image if no image is defined in the post's front matter -->
                <img src="/asset/images/placeholder.jpg" alt="Placeholder image for {{ post.title }}" class="w-full h-48 object-cover bg-gray-200 flex items-center justify-center text-gray-500 text-sm">
                {% endif %}
            </a>
        <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
        <p>
            {{ post.excerpt }}
        </p>
{% endfor %}  
</div>