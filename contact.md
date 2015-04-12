---
layout: default
title: Contact
nav: 3
permalink: /contact/
---

<h1> Let's get in touch.</h1>

{% for social in site.data.social %}
<div class="social-box">
    <a href="{{ social.url }}">
        <img src="{{ social.img }}">
    </a>
</div>
{% endfor %}
