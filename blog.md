---
layout: default
title: Blog
nav: 4
permalink: /blog/
---
<ul class="media-list">
{% for post in site.posts %}
    <li class="media">
        <div class="media-left">
            <a href="{{ post.url }}">
                <img class="media-object" src="{{ post.image }}">
            </a>
        </div>
        <div class="media-body">
            <h4 class="media-heading">
                <a href="{{ post.url}}">
                    {{ post.title}}
                </a>
            </h4>
            <h5 class="media-heading">
                {{ post.date | date: "%B %d, %Y" }}
            </h5>
            {% if post.description %}
                {{ post.description }}
            {% else %}
                {{ post.content | strip_html | truncate: 25, '...' }}
            {% endif %}
        </div>
    </li>
{% endfor %}
</ul>