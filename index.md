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

<figure class="third">
  {% for post in site.frettir limit:3 %}
    <a href="{{ post.url |relative_url }}" style="text-decoration:none;">
      {% if post.header.teaser %}
        <img src="{{ site.baseurl  }}{{post.header.teaser}}">
      {% endif %}
      {{post.title}}
      <span style="display:block; margin:0 0 20px; font-size:80%; color:grey;">{{ post.date | date:"%Y-%m-%d" }}</span>
    </a>
  {% endfor %}
</figure>

<a href="/frettir/" class="btn btn-purple" style="display:block; margin: auto; width:200px; font-size:1em">Allar fréttir</a>

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

### All posts (20)

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

### All pages (20)
{% for page in site.pages limit: 20 %}
   <a href="{{ site.baseurl }}{{ page.url }}">{{ page.title }}</a>
{% endfor %}


