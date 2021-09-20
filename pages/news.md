---
title: News
---

<a href="/news.xml"><i class="fas fa-rss fs-1"></i></a>
<br/>
<ul class="list-unstyled">
    {%- for post in site.news reversed -%}
    <li>    
    <h4 class="mt-1">
        <a href="{{ post.url | relative_url }}">
        {{ post.title | escape }}
        </a>
    </h4>
    
    <span class="text-muted">        
        <time datetime="{{ post.date | date_to_xmlschema }}">
           {{ post.date | date: site.date_format }}</time>
    </span>
    
    {%- if site.show_excerpts -%}
        {{ post.excerpt }}
    {%- endif -%}
    </li>
    {%- endfor -%}
</ul>

<p class="rss-subscribe">subscribe <a href="{{ '/feed.xml' | relative_url }}">via RSS</a></p>