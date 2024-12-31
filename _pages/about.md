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

As a dual major in Mechanical Engineering and Robotics at Carnegie Mellon University, I bring 8+ years of hands-on experience in mechanical design, electrical systems, programming, and manufacturing. My expertise spans CAD modeling, robotic systems, numerical analysis, and mentoring future engineers.

Currently, I serve as the Mechanical Team Lead for CMU's Robosub team and TA for Howie Choset's renowned Introduction to Robotics course. My passion lies in pioneering technologies like biofuel ship cleaning, 3D printing, and advanced manufacturing, with prior impactful work in agricultural robotics.

<br>
<h1>

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
