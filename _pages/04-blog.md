---
title: Blog
layout: splash
permalink: /blog
header:
    overlay_image: /images/splash/webdev.jpg
    caption: "Photo credit: [**Unsplash**](https://unsplash.com)"
    overlay_filter: rgba(0, 0, 0, 0.6)
excerpt: "**Lorem Ipsum**"
---

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>