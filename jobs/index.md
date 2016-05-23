---
title: Jobs
---
<ul class="post-list">

<h1 style="color: #000000;">
</h1>

<h2 style="color: #000000;">
  Work at the Sustainable Engineering Lab
</h2>

<p style="color: #000000;">
  We solve real-world problems in the developing world; we use engineering to make the development process smarter and to bring new services, like health and energy, to people that need them most. 
</p>

<p style="color: #000000;">
  <em>Columbia University is an affirmative action/equal opportunity employer. Minorities and women are encouraged to apply.</em>
</p>

<h2 style="font-weight: 500 !important; color: #000000;">
  Current opportunities:
</h2>
  {% for post in site.categories.jobs %}
      <h1>
        {{ post.title }}
      </h1>
      <p>{{post.content}}</p>
  {% endfor %}
</ul>
<h2 style="font-weight: 500 !important; color: #000000;">Projects</h2>
<p style="color: #000000;">Have a look around our site for some of the <a href="/projects/">projects</a> we are working on, and some <a href="/products-tools/">software tools</a> we are building to solve the problems we encounter.</p>
<p style="color: #000000;">Project examples:</p>

<ul style="color: #000000;">
	<li>Nigeria Scale-up Initiative &#8211; Taking the lessons of the Millennium Villages (http://www.millenniumvillages.org/) to scale in a partnership with Nigeria&#8217;s Presidential taskforce on the Millennium Development goals. <a href="/tags/#Nigeria Scale-up Initiative">See related blog posts</a></li>
	<li><a href="/dristhi/">Dristhi</a> &#8211; Mobile-based patient tracking for rural nurse midwives.</li>
	<li><a href="/smart-solar-irrigation/">Solar Irrigation</a> &#8211; Smart solar irrigation in Senegal.</li>
</ul>
