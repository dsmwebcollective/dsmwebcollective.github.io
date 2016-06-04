---
layout: page
title: Des Moines User Groups
nav_title: User Groups
permalink: /user-groups/
---

<ul class="list groups-list">
    {% if site.data.groups %}
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

        <li>
            <a href="#" target="_blank">Have a user group to add?</a>
        </li>
    {% else %}
        <li>
            No user groups at this time. <a href="#" target="_blank">Have a user group to add?</a>
        </li>
    {% endif %}
</ul>
