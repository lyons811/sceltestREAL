---
title: "News"
layout: default
permalink: /news/
---

# All News

<table>
{% for post in site.posts %}
  <tr>
    <td>
    <span style="display:inline-block; padding-right:20px;">
    {{ post.date | date: "%b %-d, %Y" }}
    </span>
    <a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
    </td>
    <br />
  </tr>
{% endfor %}
</table>
