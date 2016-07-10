---
layout: default
permalink: /projects/
---
# $ cat projetcs.txt
None done yet, but we would like to work on some cool projects together
if you have any suggestions or want to work on a project together please
hop on to the [mailing list.](mailto:codingclub-discussoins+subscribe@googlegroups.com)

# $ cat /proc/projects
<ul>
    {% for project in site.projects %}
        <li> 
            <h2><a href="{{ project.url }}">{{ project.title }}</a></h2>
            {{ project.excerpt }}
        </li>
    {% endfor %}
</ul>
