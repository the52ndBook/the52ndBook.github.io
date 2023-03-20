---
layout: page
title: A (not so) short collection of pubquiz questions
---

## A normal title 

Some other text here

<p>
{% for item in site.data.questions %}
    {% if item.category == 'literature' %}
        <p> <b>Question:</b> {{ item.question }} </p>
        <p> <b>Answer:</b> <i> {{ item.answer }} </i>  </p> <br>
    {% endif %}
{% endfor %}
<p>
