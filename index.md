---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: Solutions for Online Publishing and Communities
is_home: true
---
# Colette Snow Media creates solutions for online publishing and communities. Our focus is on building usable and accessible solutions to help you succeed

## Products

<div class="latest-products">

<div class="product">

<p class="product-title"><a href="/products/bulk-user-management"><strong>Bulk User Management</strong></a></p>
<p class="csm_price">WordPress Plugin | Free</p>

<p>WordPress plugin to allow bulk importing, editing, and deletion of users via the use of <abbr title="Comma Separated Value">CSV</abbr> files.</p>
</div>
</div>

## Latest Blog Posts

<div class="latest-posts">
{% for post in site.posts limit: 3 %}
  <article class="post">
    <div class="post_details">
        <p>{{ post.date | date: "%b %-d, %Y" }}</p>
        <h3 class="entry-title">
            <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
        </h3>
        <p>{{- post.excerpt | strip_html }}  <small><a href="{{ post.url | prepend: site.baseurl }}">Read More&hellip;</a></small></p>
        <div class="post_meta"><a href="{{ post.url | prepend: site.baseurl }}#disqus_thread">Comments</a></div>
    </div>

  </article> 
{% endfor %}
</div>