---
layout: about
---

<h1>About</h1>

<p class="abouttext">My name is Rita and I'm a UX/UI designer from Lisbon, Portugal. I consider myself a detail-oriented problem-solver and I always love new challenges. I really love the bond that we can create between art and technology.</p>

<p class="abouttext">I look at design as a means of finding solutions that solve a certain need in an accessible and sustainable way. Throughout my work process, I focus on human-centered design to build innovative products that answer people's needs. I'm also a firm believer that good and bad feedback are both equally important for our personal and professional growth.</p>

<h2>Experience</h2>

<ul class="details">
    {% for workexperience in site.experience %}
        <li><h3>{{ workexperience.title }}</h3></li>
        <li><p>{{ workexperience.category }}</p></li>
        <li><p>{{ workexperience.duration }}</p></li>
        
    {% endfor %}
</ul>

<h2>Education</h2>

<ul class="details">
    {% for courses in site.education reversed %}
        <li><h3>{{ courses.title }}</h3></li>
        <li><p>{{ courses.category }}</p></li>
        <li><p>{{ courses.duration }}</p></li>
    {% endfor %}
</ul>

<h2>{{ site.data.skills.docs_list_title }}</h2>

<ul class="details">
    {% for skill in site.data.skills.docs %}
        <li>{{ skill.title }}</li> 
    {% endfor %}
</ul>

<h2>{{ site.data.interests.docs_list_title }}</h2>

<ul class="details">
    {% for interest in site.data.interests.docs %}
        <li>{{ interest.title }}</li> 
    {% endfor %}
</ul>