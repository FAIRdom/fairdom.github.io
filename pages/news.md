---
layout: page
title: News
---

<div class="float-right">
<a href="/news.xml">
{% octicon rss height:32 %}
</a>
</div>
<br/>

<ul class="list-unstyled">
    {%- for post in site.news reversed -%}
    <li>
    <span class="text-muted">
        {%- assign date_format = "%b %-d, %Y" -%}
        {{ post.date | date: date_format }}
    </span>
    <p class="h5">
        <a href="{{ post.url | relative_url }}">
        {{ post.title | escape }}
        </a>
    </p>
    {%- if site.show_excerpts -%}
        {{ post.excerpt }}
    {%- endif -%}
    </li>
    {%- endfor -%}
</ul>

<p class="rss-subscribe">subscribe <a href="{{ '/feed.xml' | relative_url }}">via RSS</a></p>