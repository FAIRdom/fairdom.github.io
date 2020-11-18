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
  {% assign reversed = site.news | reverse %}
  {% for news in reversed %}
    <li>
      <h4><a href="{{ news.url }}">{{ news.title | escape }}</a></h4>
      <p class="text-muted text-info">
        <time datetime="{{ news.date | date_to_xmlschema }}">
                            {{ news.date | date: site.date_format }}
                        </time>                           
      </p>      
    </li>
  {% endfor %}
</ul>