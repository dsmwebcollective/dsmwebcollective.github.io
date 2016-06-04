---
layout: page
title: Jobs in Des Moines
nav_title: Jobs
permalink: /jobs/
---

<ul class="list jobs-list">
    {% if site.data.jobs %}
        {% for job in site.data.jobs %}
            <li>
                <div class="title">
                    <span class="group">[{{ job.company }}]</span><br>
                    <a href="{{ job.url }}" target="_blank">{{ job.title }}</a>
                </div>
            </li>
        {% endfor %}

        <li>
            <a href="#" target="_blank">Have a job posting to add?</a>
        </li>
    {% else %}
        <li>
            No job postings at this time. <a href="#" target="_blank">Have a job posting to add?</a>
        </li>
    {% endif %}
</ul>
