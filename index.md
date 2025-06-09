---
title: Welcome to my blog
---
Tom's Saleforce Blog

{% for post in site.posts %}  
    <div>
        <a href="{{ site.baseurl }}{{ post.url }}" class="block">
                <!-- Post Image -->
                {% if post.image %}
                <img src="{{ post.image | relative_url }}" alt="{{ post.title }}" class="w-full h-48 object-cover">
                {% else %}
                <!-- Placeholder image if no image is defined in the post's front matter -->
                <img src="https://placehold.co/600x400/22c55e/ffffff?text=No+Image" alt="Placeholder image for {{ post.title }}" class="w-full h-48 object-cover bg-gray-200 flex items-center justify-center text-gray-500 text-sm">
                {% endif %}
            </a>
        <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
        <p>
            {{ post.excerpt | strip_html | truncatewords: 30 }}
        </p>
    </div>

{% endfor %}  