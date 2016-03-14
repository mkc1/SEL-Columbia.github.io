---
id: 20
title: Projects
author: jonathan-carbajal
guid: http://modilabs.org/?page_id=20
---

<div class="container">
<h1>Sustainable Energy Projects</h1>
{% for project in site.categories.projects %}
    {% if project.type == 'Sustainable Energy' %}
        <div class="row-fluid projects">
            {% include project_summary.html post=project %}
        </div>
    {% endif %}
{% endfor %}

<h1>ICT4D & Development Planning Projects</h1>
{% for project in site.categories.projects %}
    {% if project.type == 'ICT4D and Development Planning' %}
        <div class="row-fluid projects">
            {% include project_summary.html post=project %}
        </div>
    {% endif %}
{% endfor %}
</div>
