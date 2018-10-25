---
permalink: /frettir/
title: Fréttir
---

## 20 Fréttir
<div class="row">
  {% for post in site.frettir limit: 20 %}
  <div class="col-sm-6 col-md-4 ">
    <div class="card">
      <a href="{{ site.baseurl }}{{ post.url }}">
        <img class="card-img-top" src="{{ site.baseurl }}{{ post.image }}" />
        <h5 class="p-3 text-center"> {{ post.title }} </h5>
      </a>
      <div class="card-body">
        <span>{{ post.date | date:"%Y-%m-%d" }}</span>
      </div>
    </div>
  </div>
  {% endfor %}
</div>
