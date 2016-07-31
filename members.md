---
layout: default
permalink: /members/
---
# Members of Coding Club .... 
{:style="text-align: center"}

<div class="member-container">
{% assign members = site.data.members %}
{% for member in members %}
<div class="members">
    {% for info_fields in  member[1] %}
        <a href="https://twitter.com/{{ info_fields.twitter }}"><img src="{{ info_fields.avatar }}" class="member-avatar" alt="{{ info_fields.name }}" /> </a><br/>
        {{ info_fields.name }} <br/>
        github:<a href="https://github.com/{{ info_fields.github }}"> {{ info_fields.github }} </a><br/>
        email:{{ info_fields.email }} <br/>
</div>
    {% endfor %}
{% endfor %}
</div>
