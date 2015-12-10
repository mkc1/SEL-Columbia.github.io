---
title: About
layout: default
---

{% for post in site.categories.about %}

<div class="row">
  <div class="col-md-9 col-lg-6 col-sm-12"> 
    <h2>{{ post.title }}</h2>
    <p>{{ post.content }}</p> 
  </div>
</div>

{% endfor %}

<!-- Current Members (team) -->

<div class="row-fluid">
  <div class="span9">
    <h2>
      Team
    </h2> The Lab brings together a diverse set of talents who work in collaboration to engineer solutions to development issues. From designers who understand user needs and talented software engineers to development practitioners and researchers, the expertise at the lab is both broad and deep.
  </div>
</div>

{% for member in site.categories.team reversed %}
{% cycle 'add rows': '<div class="row">', nil, nil, nil %}
<div class="col-md-3">
    <div class="media">
        <a class="pull-left" href="{{ member.url }}">
        <img class="media-object" src="{{ member.photo }}">
        </a>
        <div class="media-body">
            <div class="head media-heading"><a href="{{ member.url }}" class="off">{{ member.full_name}}</a></div>
            <p class="note">{{ member.title }}</p>
        </div>
    </div>
</div>    
{% cycle 'close rows': nil, nil, nil, '</div>' %}
{% endfor %}
{% cycle 'close rows': nil, '</div>', '</div>', '</div>' %}

<!-- Alumni -->

<div class="row-fluid">
  <div class="span9">
    <h2>
      Alumni 
    </h2>  </div>
</div>

{% for alum in site.categories.alumni reversed %}
<div class="row">
    <div class="col-md-2">
        {{ alum.full_name }}
    </div>
    <div class="col-md-2">
        {{ alum.employer }}
    </div>
</div>

{% endfor %}
