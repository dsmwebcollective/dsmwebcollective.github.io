---
layout: page
title: Events
heading: Explore Upcoming Events
permalink: /events/
---

<ul>
    {% for event in site.event %}
        <li>
            <h2><a href="{{ event.url }}">{{ event.title }}</a></h2>
            <p>Event Date: {{ event.event_date | date: "%b %-d, %Y at %l:%M%p" }}</p>
        </li>
    {% endfor %}
</ul>
