---
layout: page
title: Jobs
heading: Jobs in Des Moines
permalink: /jobs/
---

<ul class="list jobs-list">
    {% for job in site.data.jobs %}
        <li>
            <div class="title">
                <span class="group">[{{ job.company }}]</span><br>
                <a href="{{ job.url }}" target="_blank">{{ job.title }}</a>
            </div>
        </li>
    {% endfor %}
</ul>
