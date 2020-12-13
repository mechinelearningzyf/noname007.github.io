---
layout: page
title: PHP
permalink: /tags-php/
published: true
---



<div class="blog-tags"> 
    {% assign tags = site.tags | sort %}
	{% for tag in tags %} 
	{% if tag[0] == "php" %} 
		{% for post in tag[1] %}
			<a class="post-subtitle" href="{{ site.baseurl }}{{ post.url }}">
				<li>
					{{ post.title }}	<small class="post-meta"> - Posted on {{ post.date | date: "%B %-d, %Y" }}</small>
				</li>
			</a>
        {% endfor %}
		{% endif %}
    {% endfor %}
</div>
