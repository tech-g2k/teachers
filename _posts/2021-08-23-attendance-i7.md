---
layout: post
title: "Attendance i7"
---

Attendance sheets for all the classes . . .

<div class="wrap">
    <ul style="list-style: none;">
        {% for item in site.data.attendance-i7 %}
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
