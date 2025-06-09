---
title: Home Page Content 
---
<head>
<style>
p.big {
  line-height: 1.8;
}
</style>
</head>
<body>

<div>
{% for post in site.posts %}
        <a href="{{ site.baseurl }}{{ post.url }}">
                <!-- Post Image -->
                {% if post.image %}
                <img src="{{ post.image | relative_url }}" alt="{{ post.title }}">
                {% else %}
                <!-- Placeholder image if no image is defined in the post's front matter -->
                <img src="assets\images\placeholder.jpg" alt="Placeholder image for {{ post.title }}">
                {% endif %}
            </a>
        <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
            <p class="big">
                {{ post.excerpt }}
            </p>
{% endfor %}  
</div>

