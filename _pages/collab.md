---
title: "Collaborator Projects"
permalink: /projects/collab/
---

{% assign collab_projects = site.static_files | where_exp: "file", "file.path contains '_projects/collab'" %}

{% for project in collab_projects %}
  <div class="project">
    <h2>{{ project.name }}</h2>
    <p><a href="{{ project.path }}">View file</a></p>
  </div>
{% endfor %}
