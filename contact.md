---
layout: contacts
---

<h1>Contacts</h1>

<h2>
    <a href="mailto: rita.dupereira@gmail.com" target="_blank" title="E-mail">rita.dupereira@gmail.com</a>
</h2>

<ul>
   {% for contact in site.mycontacts %}
      <li>
        <a href="{{ contact.link }}" target="_blank" title="{{ contact.link-title }}">
        {{ contact.link-title }}
        </a>
      </li>
   {% endfor %}
</ul>>