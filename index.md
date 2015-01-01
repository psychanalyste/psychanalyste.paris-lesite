---
layout: archive
permalink: /
title: "Psychanalyste.Paris - Découvrir"
excerpt: "Sur la Psychanalyse."
image:
  feature: home-feature.jpg
id: home
---

Heureusement la psychanalyse n'est pas la seule façon de résoudre les conflits internes. La Vie elle-même reste un bon thérapeute.
{:.shorten}

---

### [Paper for iPad Tips & Tricks]({{ site.url }}/mastering-paper/)

<div class="tiles">
{% for post in site.categories.mastering-paper limit:4 %}
	{% include post-grid.html %}
{% endfor %}
</div><!-- /.tiles -->

---

### [Words I've Written]({{ site.url }}/articles/)

<div class="tiles">
{% for post in site.categories.articles limit:4 %}
  {% include post-grid.html %}
{% endfor %}
</div><!-- /.tiles -->

---

### [Portraits I've Drawn]({{ site.url }}/paperfaces/)

<ul class="th-grid-full">
{% for post in site.categories.paperfaces limit:8 %}
  <li><a href="{{ site.url }}{{ post.url }}" title="{{ post.title }}"><img src="{{ site.url }}/images/{{ post.image.thumb }}" alt="thumbnail image"></a></li>
{% endfor %}
</ul>