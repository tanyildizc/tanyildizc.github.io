---
title: notes
layout: page
nav: custom
custom-nav: 
    - '<a href="/about" title="about">about</a>&nbsp;|&nbsp;'
    - '<a href="/blog" title="blog">blog</a>&nbsp;|&nbsp;'
    - '<a href="/contact" title="contact">contact</a>'
permalink: /notes
---

<div class="callout" markdown="1">

## what are notes?

this is a microblog for frequent, shorter thoughts, interesting links and shaping ideas before they become full posts. the best way to follow is via [the rss feed](/rss).

</div>


{% for post in site.categories.notes limit: 10 %}
<section class="note-entry" markdown="1">
<h1><a href="{{post.url}}" style="text-decoration: none;">{{post.title}}</a></h1>

{{post.content}}

<p class="note-date-line"><time datetime="{{ post.date | date: '%Y-%m-%d' }}">{{ post.date | date: "%B %d, %Y" }}</time></p>
</section>


{% endfor %}

<div class="callout" markdown="1">

## you’ve reached the end, kind of

notes are meant to be fleeting, so i only display the last 10 of them. older notes are still accessible either via their respective permalink or the [random note](/notes/random) link.

</div>


