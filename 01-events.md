---
layout: list
title: Upcoming Events
nav_title: Events
permalink: /events/
---

<div class="list list-animate events-list">
    {% if site.data.events %}
        {% for event in site.data.events %}
            <a href="{{ event.details_url }}" target="_blank">
                <div class="date">
                    {% assign new_date = event.date | split: " " %}
                    {{ new_date[0] }}
                    <div class="day">{{ new_date[1] }}</div>
                </div>

                <div class="content">
                    {% if event.group %}
                        <div class="group">[{{ event.group }}]</div>
                    {% endif %}

                    <div class="title">
                        {{ event.title }}</a>
                    </div>

                    <div class="time">
                        {{ event.time }} ({{ event.location }})
                    </div>
                </div>
            </a>
        {% endfor %}

        <a href="https://github.com/dsmwebcollective/dsmwebcollective.github.io/blob/master/CONTRIBUTING.md" target="_blank">Have an upcoming event to add?</a>
    {% else %}
        <a href="https://github.com/dsmwebcollective/dsmwebcollective.github.io/blob/master/CONTRIBUTING.md" target="_blank">No upcoming events at this time. Have an upcoming event to add?</a>
    {% endif %}
</div>
