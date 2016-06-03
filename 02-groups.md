---
layout: page
title: User Groups
heading: Des Moines User Groups
permalink: /user-groups/
---

<ul class="list groups-list">
    {% for group in site.data.groups %}
        <li>
            <div class="title">
                <a href="{{ group.url }}" target="_blank">{{ group.title }}</a>
            </div>

            {% if group.meeting %}
                <div class="group">Meetings: {{ group.meeting }}</div>
            {% endif %}
        </li>
    {% endfor %}
</ul>
