---
id: 20
title: Projects
author: jonathan-carbajal
guid: http://modilabs.org/?page_id=20
---

<div>
<h2 id="sustainable_energy_projects">Sustainable Energy Projects</h2>
{% for project in site.categories.projects %}
    {% if project.type == 'Sustainable Energy' %}
        <div class="row-fluid projects">
            <div class="span12">
                {% include project_summary.html post=project %}
            </div>
        </div>
    {% endif %}
{% endfor %}

<h2>ICT4D & Development Planning Projects</h2>
{% for project in site.categories.projects %}
    {% if project.type == 'ICT4D and Development Planning' %}
        <div class="row-fluid projects">
            {% include project_summary.html post=project %}
        </div>
    {% endif %}
{% endfor %}
</div>
