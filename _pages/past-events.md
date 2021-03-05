---
layout: page
title: Past Events
---

{% include event-visibility-javascript.html %}

{% include calendar-button.html %}

<br/>

{% include event-list.html -%}

<script>
    $(document).ready(function() {
        showEventsBeforeNow();
        $('#calendar-button').show();
    });
</script>
    