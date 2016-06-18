---
layout: default
---
# $ cat meetups.txt
we organise meetups to discuss about various topics whenever possible,
we fix the time and place for this meetings on our mailing list. Subscribe
to the list to get informed when we will meet next.

# $ cat /proc/meetups
<ul>
    {% for meetup in site.meetups %}
        <li> 
            <a href="{{ meetup.url }}">{{ meetup.title }} on {{ meetup.date | date_to_string }}</a>
            {{ meetup.excerpt }}
        </li>
    {% endfor %}
</ul>
