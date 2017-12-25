---
permalink: /events/
layout: archive
title: "Events"
author_profile: false
---

All events are free and open to the public. Click an event below for
details.

# Upcoming Events

{% assign planned = site.planned_events %}
{% if planned.size > 0 %}
  {% for post in planned %}
    {% include archive-single.html %}
  {% endfor %}
{% else %}
  _No events planned at this time! But stay tuned._
{% endif %}

# Past Events

{% assign past = site.past_events | reverse %}
{% for post in past %}
  {% include archive-single.html %}
{% endfor %}
