---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: splash
header:
  image: /assets/images/karoline_fund_piratar_banner-wide.jpg
  caption: 'Framtidin okkar'
  image_description: 'Lysing myndar'
---

# Fréttir

<ul class="">
{% for post in site.frettir limit: 3 %}
  <div class="">
    <li>
         <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
         <span>({{ post.date | date:"%Y-%m-%d" }})</span>
         <p>{{post.excerpt}}</p>
    </li>
  </div>
{% endfor %}
</ul>
<a href="/frettir/" class="btn btn-purple">Allar fréttir</a>

<hr />
3 horiz. columns
- Nýjast í kosningakerfi
- Vidburdadagatal
- Taktu þátt

<hr />
### Stefnumalin
4 horiz. columns
- Heilbrigðiskerfið
- Húsnæðismál
- Hækkum persónuafslátt
- Tjáningarfrelsi

<hr />
## Frambjodendur

<hr />
3 horiz. columns
- Grasrót Pírata
- Stefnur
- Styrktu Pírata

<hr />
# Píratar í fjölmiðlum

<hr />
# Samfélagsmiðlar

Viljum vid ad forsidan hladi upp instagram og fb i hvert skipti?

<hr />
<hr />
<hr />

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


