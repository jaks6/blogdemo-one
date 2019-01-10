---
site.title : Jakob's Blog
---


## Post List

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | prepend:site.baseurl }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>

## Tag list
  <ul class="tag-cloud">
{% for tag in site.tags %}
  <li>
  		<a href="{{ site.baseurl }}/tags#{{ tag[0] | slugize }}">
        {{ tag[0] }}
      </a>
  </li>
  {% endfor %}
</ul>
