---
layout: page
title: Posts List
header: Posts By Category
group: navigation
---

<div class="col-md-12 col-sm-12 col-xs-12">
    <ul class="list-unstyled">
        {% for post in site.posts %}
        <li>
            <span>
                {{ post.date | date_to_string }} &raquo;
            </span>
            <span>
                <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a>
            </span>
        </li>
        {% endfor %}
    </ul>
</div>

<div class="clearfix"></div>
