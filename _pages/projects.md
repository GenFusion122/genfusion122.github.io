---
title:
layout: default
permalink: /
published: true
---
# Projects
<div class="ProjectContainer">
	<div class="gallery">
  {% for project in site.projects %}
  <div class="projectTile">
    <a href="{{ project.url | prepend: site.baseurl | prepend: site.url }}">
      <div class="projectImage">
      <img class="projectImage" src="{{ project.image }}" alt="asd">
        <div class="overlay">
            <div class="text">{{ project.description }}</div>
        </div>
      </div>
          <span>
              <h2>{{ project.title }}</h2>
          </span>
          </a>
  </div>

  {% endfor %}

	</div>

</div>
