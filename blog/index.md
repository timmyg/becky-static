---
id: 415
title: Articles all
date: 2011-06-23T14:02:09+00:00
author: Becky Barras
layout: page
guid: ?page_id=415


---
<h2 class="blog-blurb">
  My personal and professional lifestyle will be featured in my blog. Join me in this journey of creativity, celebration and humor.!
</h2>
{% for post in site.posts %}
  <article id="post-512" class="post-512 post type-post status-publish format-standard has-post-thumbnail hentry category-uncategorized cat-1-id">
      <header>
        <h2><a href="{{ post.url }}" title="{{ post.title }}" rel="bookmark">{{ post.title }}</a></h2>
        <div class="post-meta"></div>
      </header>
      <div class="featured-thumbnail"><img width="188" height="125" src="{{ post.hero_img }}" class="attachment-post-thumbnail wp-post-image" alt="red door hb"></div>      <div class="post-content">
        <div class="excerpt">{{ post.excerpt | strip_html }}</div>
        <div class="clear"></div>
        <a href="{{ post.url }}" class="link">Read More</a>
      </div>
    <footer></footer>
    </article>
{% endfor %}
