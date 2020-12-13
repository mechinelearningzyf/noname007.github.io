---
layout: page
title: 技术随笔
permalink: /tags-techs-notes/
published: true
---

<div class="blog-tags"> 
    {% assign tags = site.tags | sort %}
	{% for tag in tags %} 
		{% if tag[0]=="工具" or tag[0] == "技术" %}
		{% for post in tag[1] %}
			<a class="post-subtitle" href="{{ site.baseurl }}{{ post.url }}">
				<li>
					{{ post.title }}	<small class="post-meta"> - {{ post.date | date: "%B %-d, %Y" }}</small>
				</li>
			</a>
        {% endfor %}
		{% endif %}
    {% endfor %}
</div>
