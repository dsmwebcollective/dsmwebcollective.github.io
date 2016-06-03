---
layout: page
title: Upcoming Events
nav_title: Events
permalink: /events/
---

<ul class="list events-list">
    {% for event in site.data.events %}
        <li>
            <div class="title">
                <span class="group">[{{ event.group }}]</span><br>
                <a href="{{ event.details_url }}" target="_blank">{{ event.title }}</a>
            </div>

            <div class="date">
                {{ event.date }} @ {{ event.time }} ({{ event.location }})
            </div>
        </li>
    {% endfor %}
</ul>
