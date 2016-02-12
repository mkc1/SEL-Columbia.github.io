---
title: Blog
layout: default
---

<div class="container">
    {% for post in site.categories.blog limit: 8%}
        <div class="row">
            <h2>
                <a href="{{ post.url | prepend: site.baseurl }}">
                  <img class="first-image-thumbnail alignnone size-large wp-image-4513" src="{{ post.image | prepend: site.baseurl }}" alt="Water Pump" width="700" height="238" /></a>
                  <br>
                  {{ post.content | strip_html | truncatewords: 50 }}
                  <br>
                  <a href="{{ post.url | prepend: site.baseurl }}" style="text-transform:uppercase; font-size: 13px; font-weight: 700;">Continue Reading »</a>
              </div>

          </article>
      </div>


      {% endfor %}
  </div>
                    {{ post.title }}
                </a>
            </h2>
            
            <p>
                <span class="article-author">
                    {{ post.author }}
                </span>
                <span class="article-date">
                    {{ post.date | date: "%b %-d, %Y"}}
                </span>
            </p>
            
            <p>
                {{ post.content | strip_html | truncatewords: 50 }}
            </p>
        </div>
</div>