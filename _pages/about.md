---
layout: about
title: about
permalink: /
subtitle: email∶<a href='cole.r.herber@gmail.com'>cole.r.herber@gmail.com</a>
display_categories: [in-progress, finished]
profile:
  align: right
  image: prof_pic.png
  image_circular: true # crops the image to make it circular
  more_info: >

news: false # includes a list of news items
selected_papers: false # includes a list of papers marked as "selected={true}"
social: false # includes social icons at the bottom of the page
---

According to all known laws of aviation, there is no way a bee should be able to fly. Its wings are too small to get its fat little body off the ground. The bee, of course, flies anyway because bees don’t care what humans think is impossible.

Yellow, black. Yellow, black. Yellow, black. Yellow, black. Ooh, black and yellow! Let’s shake it up a little. Barry! Breakfast is ready! Coming! Hang on a second. Hello? Barry? Adam? Can you believe this is happening? Yes, I know! I’m excited!

Wow! College! We’re finally graduating. Three days of grade school, three days of high school. Those were awkward. Three days of college, I’m glad I took a day off in the middle and just hiked around the hive. You did come back different.

<h1>
<br>
<br>

<a href="/projects/">A random sampling of projects

<h1>
<div class="projects">
{% if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
  {% for category in page.display_categories %}
  <a id="{{ category }}" href=".#{{ category }}">
    <h2 class="category">{{ category }}</h2>
  </a>
  {% assign categorized_projects = site.projects | where: "category", category %}
  {% assign shuffled_projects = categorized_projects | sample: 3 %}
  {% assign sorted_projects = shuffled_projects | sort: "importance" %}
  <!-- Generate cards for each project -->
  {% if page.horizontal %}
  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for project in sorted_projects %}
      {% include projects_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
  {% endif %}
  {% endfor %}

{% else %}

<!-- Display projects without categories -->

{% assign shuffled_projects = site.projects | sample: 3 %}
{% assign sorted_projects = shuffled_projects | sort: "importance" %}

  <!-- Generate cards for each project -->

{% if page.horizontal %}

  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for project in sorted_projects %}
      {% include projects_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
  {% endif %}
{% endif %}
</div>
