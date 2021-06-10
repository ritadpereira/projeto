---
layout: work
title: Selected Work
---

<h1>{{ page.title }}</h1>

<h2>UX & UI Design</h2>

<ul>
    {% for project in site.selectedwork reversed %}
        {% if project.category == "UX & UI Design" %}
        <hr>
        <li class="worklist">
            <a href= "{{ project.link }}" target="_blank" title="{{ project.title }}"> 
            {{ project.title }}
            <figure>
                <img src="{{ project.image-src }}" alt="{{ project.image-alt }}">
            </figure>
            </a>
        </li>
        {% endif %}
    {% endfor %}
</ul>

<h2 class="divider">Digital Illustration</h2>

<ul>
    {% for project in site.selectedwork %}
        {% if project.category == "Digital Illustration" %}
        <hr>
        <li class="worklist">
            <a href= "{{ project.link}}" target="_blank" title="{{ project.title }}"> 
            {{ project.title }}
            <figure>
                <img src="{{ project.image-src }}" alt="{{ project.image-alt }}">
            </figure>
            </a>
        </li>
        {% endif %}
    {% endfor %}
</ul>