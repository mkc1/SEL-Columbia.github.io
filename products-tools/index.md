---
title: 'Products &#038; Tools'
---
## While working on projects that create positive impact in the developing world, we produce open source tools and products that we release for others to use: {#products__tools}
{% for post in site.categories.products-tools %}
<div class="row-fluid products">
  <div class="col-md-12">
    <div class="row-fluid">
      <div class="col-md-4">
        <a href="{{post.image-link}}">
          <img src="{{post.image-source}}" width="{{post.image-width}}" 
           height="{{post.image-height}}" class="alignnone size-full" />
        </a>
      </div>
      <div class="col-md-8">
        {{ post.content }}
      </div>
    </div>
  </div>
</div>
{% endfor %}
