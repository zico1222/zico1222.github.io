---
layout: page
title: Author
---
{% include JB/setup %}

<script type="text/javascript" language="javascript" src="/contact.js"></script>

## {{ site.author.alias }}

- 男
- 1993/12/22 生まれ
- 電気通信大学 B3
- 東京出身・東京在住

## Contact
Gmail: <a href="JavaScript: mail_to()">{{ site.author.email }}</a>

Twitter: [zico1222](http://twitter.com/{{ site.author.twitter }})

Github: [zico1222](http://github.com/{{ site.author.github }})

## Blog
[{{ site.title }}]({{ site.url }})

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>
