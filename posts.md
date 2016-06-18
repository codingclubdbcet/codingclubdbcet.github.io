---
layout: default
---
<ul>
    {% for post in site.posts %}
        <li> 
            <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
            <i>by:</i>
            {% for author in post.authors %} 
                {% if forloop.last %} {{ author }} on {% else %} {{ author }}, {% endif %} 
            {% endfor %}
            {{ post.date | date_to_string }}
            {{ post.excerpt }}
        </li>
    {% endfor %}
</ul>
