---
permalink: /frettir/
title: Fréttir
---

## 20 Fréttir
<ul class="">
{% for post in site.frettir limit: 20 %}
  <div class="">
    <li>
         <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
         <span>({{ post.date | date:"%Y-%m-%d" }})</span>
    </li>
  </div>
{% endfor %}
</ul>

