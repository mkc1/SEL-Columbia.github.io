---
id: 20
title: Projects
author: Jonathan Carbajal
layout: page
guid: http://modilabs.org/?page_id=20
---

{% for post in site.categories.projects %}
<div class="row-fluid projects">
    <div class="col-sm-12">
        <div class="row-fluid">
            <div class="col-sm-4"><img src="http://sel.columbia.edu/wp-content/uploads/2014/12/delhi_map_300x329.png" alt="Delhi Map"></div>
            <div class="col-sm-4 projects-details">
                <h3>Delhi Energy Project</h3>
                <p>{{ post.exceprt }}</p>
                <p><a href="{{ post.url | prepend: site.baseurl }}">Read more</a></p>
            </div>
        </div>
    </div>
</div>
{% endfor %}