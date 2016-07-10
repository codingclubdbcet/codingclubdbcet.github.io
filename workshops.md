---
layout: default
permalink: /workshops/
---
# $ cat workshops.txt
we organise workshops to keep our members updated with the latest and greates technologies in the field of computer science,
to learn about new and less known subjects and to have some good time together with everyone.

# $ cat /proc/workshops
<ul>
    {% for workshop in site.workshops %}
        <li> 
            <h2><a href="{{ workshop.url }}">{{ workshop.title }} on {{ workshop.date | date_to_string }}</a>
            {{ workshop.excerpt }}
        </li>
    {% endfor %}
</ul>
