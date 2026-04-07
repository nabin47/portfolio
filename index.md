---
layout: default
title: Home
---

# Hi, I'm Your Name

I am an aspiring PhD student passionate about research in **your domain**. This portfolio highlights my research, software projects, writing, and professional experience.

## About Me {#about}

Write a concise and targeted statement for faculty admissions committees:

- Research interests and long-term goals.
- Academic background and strengths.
- Why your work matters.

## Projects {#projects}

{% for project in site.projects %}
- [{{ project.title }}]({{ project.url | relative_url }}) — {{ project.summary }}
{% endfor %}

## Publications {#publications}

{% assign publications = site.publications | sort: 'year' | reverse %}
{% for pub in publications %}
- **{{ pub.title }}** ({{ pub.year }})  
  {{ pub.authors }}  
  *{{ pub.venue }}*{% if pub.link %} · [Link]({{ pub.link }}){% endif %}
{% endfor %}

## Work Experience {#experience}

{% assign experiences = site.experience | sort: 'start' | reverse %}
{% for item in experiences %}
- **{{ item.role }}**, {{ item.org }} ({{ item.start }} – {{ item.end | default: 'Present' }})  
  {{ item.summary }}
{% endfor %}
