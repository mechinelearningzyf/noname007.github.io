---
layout: page
title: Tags
permalink: /tags-cloud/
published: true
---
<h3>My Popular Repositories</h3>
{% if site.github.public_repositories != null %}
{% assign repos = site.github.public_repositories | sort: "stargazers_count" | reverse%}
{% for repo in repos | limit: site.side_bar_repo_limit %}
<a href="{{ repo.html_url }}" target="_blank" class="card text-center">
    <div class="thumbnail">
        <div class="card-image geopattern" data-pattern-id="{{ repo.name }}">
            <div class="card-image-cell">
                <h3 class="card-title">
                    {{ repo.name }}
                </h3>
            </div>
        </div>
        <div class="caption">
            <div class="card-description">
                <p class="card-text">{{ repo.description }}</p>
            </div>
            <div class="card-text">
                <span class="meta-info" title="{{ repo.stargazers_count }} stars">
                    <span class="octicon octicon-star"></span> {{ repo.stargazers_count }}
                </span>
                <span class="meta-info" title="{{ repo.forks_count }} forks">
                    <span class="octicon octicon-git-branch"></span> {{ repo.forks_count }}
                </span>
                <span class="meta-info" title="Last updated：{{ repo.updated_at }}">
                    <span class="octicon octicon-clock"></span>
                    <time datetime="{{ repo.updated_at }}">{{ repo.updated_at | date: '%Y-%m-%d' }}</time>
                </span>
            </div>
        </div>
    </div>
</a>
{% endfor %}
{% endif %}


<div class="blog-tags"> 
    {% assign tags = site.tags | sort %}
    {% for tag in tags %}
    <a href="#{{ tag[0] | slugify }}" class="btn btn-default" style="font-size: {{ tag | last | size  |  times: 4 | plus: 80  }}%"> <!-- style="color: #1C1C1C;" is font color of cloud index -->
      <span class="fa fa-folder-open" aria-hidden="true"> 
        {{ tag[0] }} <i class="badge">{{ tag | last | size }}</i>
      </span>
    </a>
    {% endfor %}
  </div>
  <hr/> 
  <div class="post-preview"> 
    {% for tag in tags %} 
      <h2 id="{{ tag[0] | slugify }}" style="padding-top: 70px;"> {{ tag[0] }}  <i class="badge">{{ tag | last | size }}</i></h2>
      <ul class="later on">
        {% for post in tag[1] %}
          <a class="post-subtitle" href="{{ site.baseurl }}{{ post.url }}">
        <li>
          {{ post.title }}
        <small class="post-meta"> - Posted on {{ post.date | date: "%B %-d, %Y" }}</small>
        </li>
        </a>
        {% endfor %}
      </ul>
        <a href="#top" class="btn btn-default">
          <span class="fa fa-refresh" aria-hidden="true"></span> Go back to the top
        </a> 
        <hr/>
    {% endfor %}
  </div>
