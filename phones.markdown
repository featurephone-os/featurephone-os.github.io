---
layout: page
title: Phones
permalink: /phones/
---
<div id="archives">
  <div class="archive-group">
    {% capture tag_name %}Phone{% endcapture %}
    <div id="#{{ tag_name | slugize }}"></div>
    <p></p>

    <a name="{{ tag_name | slugize }}"></a>
    {% for post in site.tags[tag_name] %}
    <article class="archive-item">
      <h4><a href="{{ site.baseurl }}{{ post.url }}">{{post.title}}</a></h4>
    </article>
    {% endfor %}
  </div>
</div>
