---
title: Events

redirect_from:
    - /past-events/
    - /upcoming-events/
---


{% include event-list.html %}

<script>

/**
 * Making relevant events visible
 */
function nowToDateString() {
  return new Date().toISOString().substring(0, 10);
};

function showUpcomingEvents() {
  var dstr = nowToDateString();
  var elements = $('li.upcoming-event').filter(function () {
    return $(this).data('start') >= dstr;
  });
  elements.prepend('<span class="badge bg-primary">Upcoming</span>');
  elements.show();
};

function showPastEvents() {
  var dstr = nowToDateString();
  var elements = $('li.past-event').filter(function () {
    return $(this).data('start') < dstr;
  });
  elements.show();
};
</script>