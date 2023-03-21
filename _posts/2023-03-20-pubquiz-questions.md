---
layout: page
title: A (not so) short collection of pubquiz questions
---

In the following I list some of the questions/trivia regarding the _literature_ section.
The interested reader can contact me at [the52ndbook@gmail.com](mailto:the52ndbook@gmail.com)


<p>
{% for item in site.data.questions %}
    {% if item.category == 'literature' %}
        <p> <b>Question:</b> {{ item.question }} </p>
        <p> <b>Answer:</b> <i> {{ item.answer }} </i>  </p> <br>
        {% if item.note %}
            <p> Note from the Quizmaster: {{ item.note }}</p>
        {% endif %}
    {% endif %}
{% endfor %}
<p>
