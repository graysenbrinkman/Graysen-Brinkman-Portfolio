---
title: ""
layout: splash
author_profile: false
permalink: /projects/
---

<div style="margin-top: 1rem;">

  <h1 style="font-size: 1.8rem; font-weight: 700; margin-bottom: 2rem; color: #222;">Projects</h1>

  <!-- RESEARCH & CLUBS -->
  <div style="display: flex; align-items: center; gap: 1rem; margin-bottom: 1.5rem;">
    <span style="font-size: 0.8rem; font-weight: 600; color: #aaa; letter-spacing: 0.08em; text-transform: uppercase;">Research & Clubs</span>
    <div style="flex: 1; height: 1px; background: #e5e5e5;"></div>
  </div>

  <div style="display: grid; grid-template-columns: repeat(3, minmax(0, 1fr)); gap: 1.25rem; margin-bottom: 3rem;">
    {% assign research = site.projects | where: "section", "research" %}
    {% for project in research %}
    <a href="{{ project.url }}" style="text-decoration: none; color: inherit; border: 1px solid #e5e5e5; border-radius: 10px; overflow: hidden; display: block; transition: transform 0.2s ease, box-shadow 0.2s ease;" onmouseover="this.style.transform='translateY(-4px)';this.style.boxShadow='0 8px 24px rgba(0,0,0,0.08)';" onmouseout="this.style.transform='translateY(0)';this.style.boxShadow='none';">
      <div style="width: 100%; height: 160px; background: #eaeaea; display: flex; align-items: center; justify-content: center; color: #aaa; font-size: 0.85rem;">
        {% if project.image %}
          <img src="{{ project.image }}" alt="{{ project.title }}" style="width: 100%; height: 160px; object-fit: cover; display: block;">
        {% else %}
          Project Image
        {% endif %}
      </div>
      <div style="padding: 1.25rem;">
        <span style="font-size: 0.72rem; color: #999;">{{ project.date_range }}</span>
        <h3 style="font-size: 0.95rem; font-weight: 600; margin: 0.2rem 0 0.5rem 0; color: #222;">{{ project.title }}</h3>
        <p style="font-size: 0.82rem; color: #555; line-height: 1.5; margin: 0 0 0.75rem 0;">{{ project.description }}</p>
        <div style="display: flex; gap: 0.4rem; flex-wrap: wrap;">
          {% for skill in project.skills limit:3 %}
            <span style="font-size: 0.72rem; background: #f0f0f0; color: #555; padding: 0.2rem 0.55rem; border-radius: 20px;">{{ skill }}</span>
          {% endfor %}
        </div>
      </div>
    </a>
    {% endfor %}
  </div>

  <!-- PROJECTS -->
  <div style="display: flex; align-items: center; gap: 1rem; margin-bottom: 1.5rem;">
    <span style="font-size: 0.8rem; font-weight: 600; color: #aaa; letter-spacing: 0.08em; text-transform: uppercase;">Projects</span>
    <div style="flex: 1; height: 1px; background: #e5e5e5;"></div>
  </div>

  <div style="display: grid; grid-template-columns: repeat(3, minmax(0, 1fr)); gap: 1.25rem; margin-bottom: 3rem;">
    {% assign projects = site.projects | where: "section", "projects" %}
    {% for project in projects %}
    <a href="{{ project.url }}" style="text-decoration: none; color: inherit; border: 1px solid #e5e5e5; border-radius: 10px; overflow: hidden; display: block; transition: transform 0.2s ease, box-shadow 0.2s ease;" onmouseover="this.style.transform='translateY(-4px)';this.style.boxShadow='0 8px 24px rgba(0,0,0,0.08)';" onmouseout="this.style.transform='translateY(0)';this.style.boxShadow='none';">
      <div style="width: 100%; height: 160px; background: #eaeaea; display: flex; align-items: center; justify-content: center; color: #aaa; font-size: 0.85rem;">
        {% if project.image %}
          <img src="{{ project.image }}" alt="{{ project.title }}" style="width: 100%; height: 160px; object-fit: cover; display: block;">
        {% else %}
          Project Image
        {% endif %}
      </div>
      <div style="padding: 1.25rem;">
        <span style="font-size: 0.72rem; color: #999;">{{ project.date_range }}</span>
        <h3 style="font-size: 0.95rem; font-weight: 600; margin: 0.2rem 0 0.5rem 0; color: #222;">{{ project.title }}</h3>
        <p style="font-size: 0.82rem; color: #555; line-height: 1.5; margin: 0 0 0.75rem 0;">{{ project.description }}</p>
        <div style="display: flex; gap: 0.4rem; flex-wrap: wrap;">
          {% for skill in project.skills limit:3 %}
            <span style="font-size: 0.72rem; background: #f0f0f0; color: #555; padding: 0.2rem 0.55rem; border-radius: 20px;">{{ skill }}</span>
          {% endfor %}
        </div>
      </div>
    </a>
    {% endfor %}
  </div>

</div>