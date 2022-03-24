---
title: News
---
<div class="mb-4">
  <a href="{{ '/news.xml' | relative_url }}" class="btn bg-light hover-primary">
      <i class="fa fa-rss me-2"></i>Subscribe to the RSS feed
  </a>
</div>


<ul class="list-unstyled">
    {%- for post in site.news reversed -%}
    <li class="br-1">    
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
