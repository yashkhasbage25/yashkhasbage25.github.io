---
layout: page
permalink: /mudgala/
title: Mudgala Purana
description: Important stories from the Mudgala Purana
nav: false
---

<div class="mudgala-stories">

{% assign stories = site.mudgala %}
{% assign sorted_stories = stories | sort: "date" | reverse %}

{% for story in sorted_stories %}
    <div class="card mt-3">
        <div class="card-body">
            <h5 class="card-title">
                <a href="{{ story.url | relative_url }}">
                    {{ story.title }}
                </a>    
            </h5>
            <p class="card-text">{{ story.index }} 
            <br>
            {{ story.date | date: "%-d %B %Y" }}</p>
        </div>
    </div>
{% endfor %}

</div>
