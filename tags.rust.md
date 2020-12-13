---
layout: page
title: Rust
permalink: /tags-rust/
published: true
---



<div class="blog-tags"> 
    {% assign tags = site.tags | sort %}
	{% for tag in tags %} 
	{% if tag[0] == "rust" %} 
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

