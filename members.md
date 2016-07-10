---
layout: default
permalink: /members/
---
# Members of Coding Club .... 
<ul>
    {% assign members = site.data.members %}
    {% for member in members %}
        {% for info_fields in  member[1] %}
            {{ info_fields.name }} <br/>
            {{ info_fields.github}} <br/>
            {{ info_fields.email }} <br/>
            {{ info_fields.twitter }} <br/>
            {% endfor %}
        
    {% endfor %}
</ul>
