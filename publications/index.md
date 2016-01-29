---
title: Publications
author: Roger Wong
layout: default
---
<div>
<h1 class="page-heading">Publications</h1>

<div class="col-md-4"  style="float:left; margin:0; width:33%;">
  <h3> Infrastructure</h3>
  <ul class="post-list" style="list-style-type:none">
    {% for post in site.posts %}
      {%if post.categories contains 'publications' and post.categories contains 'Infrastructure' %}
          <li>
            <h2>
              <a class="post-link" href="{{ post.link }}" target="\_blank">{{ post.title }}</a>
            </h2>
            <p>{{post.content}}</p>
          </li>
      {% endif %}
    {% endfor %}
  </ul>
  <h3> Water</h3>
  <ul class="post-list" style="list-style-type:none">
    {% for post in site.posts %}
      {%if post.categories contains 'publications'and post.categories contains 'Water' %}
          <li>
            <h2>
              <a class="post-link" href="{{ post.link }}" target="\_blank">{{ post.title }}</a>
            </h2>
            <p>{{post.content}}</p>
          </li>
      {% endif %}
    {% endfor %}
  </ul>
</div>
<div class="col-md-4"  style="float:left; margin:0; width:33%;">
  <h3>Energy Planning</h3>
  <ul class="post-list" style="list-style-type:none">
    {% for post in site.posts %}
      {%if post.categories contains 'publications'and post.categories contains 'Energy Planning' %}
          <li>
            <h2>
              <a class="post-link" href="{{ post.link }}" target="\_blank">{{ post.title }}</a>
            </h2>
            <p>{{post.content}}</p>
          </li>
      {% endif %}
    {% endfor %}
  </ul>

  <h3>Household Energy Usage</h3>
  <ul class="post-list" style="list-style-type:none">
    {% for post in site.posts %}
      {%if post.categories contains 'publications'and post.categories contains 'Household Energy Usage' %}
          <li>
            <h2>
              <a class="post-link" href="{{ post.link }}" target="\_blank">{{ post.title }}</a>
            </h2>
            <p>{{post.content}}</p>
          </li>
      {% endif %}
    {% endfor %}
  </ul>
</div>

<div class="col-md-4"  style="float:left; margin:0; width:33%;">
  <h3>Data Collection & Analysis</h3>
  <ul class="post-list" style="list-style-type:none">
    {% for post in site.posts %}
      {%if post.categories contains 'publications'and post.categories contains 'Data Collection & Analysis' %}
          <li>
            <h2>
              <a class="post-link" href="{{ post.link }}" target="\_blank">{{ post.title }}</a>
            </h2>
            <p>{{post.content}}</p>
          </li>
      {% endif %}
    {% endfor %}
  </ul>
</div>

<p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>


</div>
