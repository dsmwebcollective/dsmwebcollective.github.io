---
layout: list
title: Des Moines User Groups
nav_title: User Groups
permalink: /user-groups/
---

<div class="list groups-list">
    {% if site.data.groups %}
        {% for group in site.data.groups %}
            <a href="{{ group.url }}" target="_blank">
                <div class="title">
                    {{ group.title }}
                </div>

                {% if group.meeting %}
                    <div class="group">{{ group.meeting }}</div>
                {% else %}
                    <div class="group">Unknown</div>
                {% endif %}
            </a>
        {% endfor %}

        <a href="https://github.com/dsmwebcollective/dsmwebcollective.github.io/blob/master/CONTRIBUTING.md" target="_blank">Have a user group to add?</a>
    {% else %}
        <a href="https://github.com/dsmwebcollective/dsmwebcollective.github.io/blob/master/CONTRIBUTING.md" target="_blank">No user groups at this time. Have a user group to add?</a>
    {% endif %}
</div>
