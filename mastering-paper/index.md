---
layout: archive
title: "Mastering Paper by FiftyThree"
excerpt: "Tutorials and techniques to help learn Paper."
modified: 2014-12-08T12:25:40-05:00
image: 
  feature: mastering-paper-feature.jpg
  thumb: paper-by-fiftythree-icon175x175.png
---

In the spirit of openness I've decided to compile everything I've learned using [*Paper by FiftyThree*](http://www.fiftythree.com), into a series of tutorials and guides titled --- Mastering Paper.
{:.shorten}

<nav class="toc toc-left">
  <ul>
    <li><h6>Getting Started with Paper</h6></li>
    <li><h6>Step by Step Paper Tutorials</h6></li>
    <li><h6>Advanced Paper Techniques</h6></li>

  </ul>
</nav><!-- /.toc-left -->

<div class="tiles tiles-right">
{% for post in site.categories.mastering-paper %}
  <article class="tile" itemscope itemtype="http://schema.org/Article">
    <a href="{{ post.url }}" title="{{ post.title }}" class="post-teaser">
      <img src="{{ site.url }}/images/preload-400.png" data-original="/images/{% if post.image.teaser %}{{ post.image.teaser }}{% else %}{{ site.teaser }}{% endif %}" class="load" alt="teaser" itemprop="image">
      <noscript><img src="/images/{% if post.image.teaser %}{{ post.image.teaser }}{% else %}{{ site.teaser }}{% endif %}" alt="teaser" itemprop="image"></noscript>
    </a>
    <h2 class="post-title" itemprop="name"><a href="{{ post.url }}">{{ post.title | remove: 'Mastering Paper by FiftyThree: ' | remove: 'Mastering Paper by 53: ' | remove: ' with Paper by 53' }}</a></h2>
    {% if post.date %}<p class="entry-date date published"><time datetime="{{ post.date | date: "%Y-%m-%d" }}" itemprop="datePublished">{{ post.date | date: "%B %d, %Y" }}</time></p>{% endif %}
    <p class="post-excerpt" itemprop="description">{{ post.excerpt | strip_html | truncate: 160 }}</p>
    </article><!-- /.tile -->
{% endfor %}
</div><!-- /.tiles-right -->