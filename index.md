---
title: "A Consortium of Services for Research Data Management and More"
search: exclude
---

**Collect**, **Manage**, **Store** and **Publish** your **data, models** and **operating procedures** in a **FAIR** manner

**[Join](https://fair-dom.org/contribute/join-us)** the hundreds of researchers who have improved research management practices in their lab, and for themselves using our software and expertise.

Or **[find out more](https://fair-dom.org/about-fairdom)** about making your research **FAIR – Findable, Accessible, Interoperable, and Re-usable**.


<iframe class="you-tube" src="https://www.youtube.com/embed/PWutnWBfUSw" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


{%- if site.news.size > 0 -%}
#### News

<ul class="list-unstyled">
{% assign news = site.news | reverse %}
{% for post in news limit:5   %}
    <li>
        <a href="{{post.url | relative_url}}">{{post.title | escape}}</a>
        <br/><small>{{ post.date | date: site.date_format }}</small>
    </li>
{% endfor %}
</ul>

For more news click [here](news)
{%- endif -%}
