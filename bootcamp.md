---
layout: page
title:  Bootcamp
permalink: /bootcamp/
---

##Hello world!

{% assign post = site.posts.first %}
<div class="c-hero" style="background: url({{post.thumbnail_image.large | relative_url}})bottom center / cover no-repeat;">
   <h1 class="c-hero__title">{{ post.title }}</h1>
   {{ post.intro | markdownify  }}
   <a href="{{ post.url }}" class="btn--hero">Read the full Post</a>
</div>