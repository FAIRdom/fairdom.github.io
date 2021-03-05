---
layout: page
title: Past Events
---

{% include event-visibility-javascript.html %}

<div class="float-right pb-1">
<a href="/calendar" class="float-right">
<button class="btn btn-outline-primary">
{% octicon calendar height:16 %} Calendar
</button>
</a>
</div>

<br/>

{% include event-list.html -%}

<script>
    $(document).ready(function() {
        showEventsBeforeNow();
    });
</script>
    