---
title: Answer Sheets
---

# Answer Sheets

Printable answer sheets for every episode.

<ul>
  {% assign sheets = site.static_files | where: "extname", ".pdf" %}
  {% for sheet in sheets %}
    {% if sheet.path contains 'assets/pdf' %}
      <li><a href="{{ sheet.path }}">{{ sheet.name }}</a></li>
    {% endif %}
  {% endfor %}
</ul>
