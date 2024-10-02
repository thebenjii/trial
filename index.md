---
layout: default
title: Home
---

# Welcome to the Internship Job App

Start your career journey with the best internship opportunities.

## Latest Internship Openings

{% for internship in site.pages %}
  {% if internship.layout == "internship" %}
  ---
  ### [{{ internship.title }}]({{ internship.url | relative_url }})

  **Company**: {{ internship.company }}

  **Location**: {{ internship.location }}

  **Description**: {{ internship.description | truncate: 100 }}

  [View Details and Apply]({{ internship.url | relative_url }})

  ---
  {% endif %}
{% endfor %}
