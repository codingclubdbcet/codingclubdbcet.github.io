---
layout: default
---
<ul>
    {% for post in site.posts %}
        <li> 
            <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
            by {% for author in post.authors %} {{ author }} {% endfor %}
            {{ post.date }}
            {{ post.excerpt }}
        </li>
    {% endfor %}
</ul>
