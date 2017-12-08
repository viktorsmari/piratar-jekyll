---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: search
header:
  image: /assets/images/karoline_fund_piratar_banner-wide.jpg
  caption: 'Piratar framtidin okkar'
  image_description: 'Lysing myndar'
---

#### (index.md) | site.baseurl: {{ site.baseurl }}

### All posts

<ul class="">
{% for post in site.posts limit: 20 %}
  <div class="">
    <li>
         <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
         <span>({{ post.date | date:"%Y-%m-%d" }})</span>
    </li>
  </div>
{% endfor %}
</ul>

### All pages
{% for page in site.pages limit: 20 %}
   <a href="{{ site.baseurl }}{{ page.url }}">{{ page.title }}</a>
{% endfor %}


