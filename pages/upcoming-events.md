---
layout: page
title: Upcoming Events
---

{% include event-visibility-javascript.html %}

{% include calendar-button.html %}

<br/>

{% include event-list.html -%}

<script>
    $(document).ready(function() {
        showEventsAfterNow();
        $('#calendar-button').show();
    });
</script>