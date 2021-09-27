---
layout: post
title: "i7 attendance"
tags: i7 attendance
all-att: 1RPevOdeCOYU22JiPCe2WpVwVTIMKtR_3J1WVdELQTPU
---

Attendance sheets for all the classes . . .

<div class="wrap">
    <ul style="list-style: none;">
        {% for item in site.data.attendance-i7_2021 %}
            <a href="{{ item.link }}" class="stitches_btn">{{ item.class }}</a>
            &nbsp; &nbsp; &nbsp; &nbsp;
            {% assign remainder = forloop.index | modulo: 2 %}
            {% if remainder == 0 %} 
                </ul>
                <ul style="list-style: none;">
            {% endif %}
        {% endfor %}
    </ul>
</div>
<br>
{% include break-line.html %}

<a href="{{ site.gdrive }}{{ page.all-att }}" class="stitches_btn">Combined i7 & i8</a>
