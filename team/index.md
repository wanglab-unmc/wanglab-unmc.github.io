---
title: Team
nav:
  order: 3
  tooltip: About our team
---

# {% include icon.html icon="fa-solid fa-users" %}Team

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis
nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.

{% include section.html %}
## Principal Investigator
{% include list.html data="members" component="portrait" filter="role == 'pi'" %}
## Postdoctoral Researchers
{% include list.html data="members" component="portrait" filter="role == 'postdoc'" %}
## Students
{% include list.html data="members" component="portrait" filter="role == 'phd'" %}
## Research Technician
{% include list.html data="members" component="portrait" filter="role == 'tech'" %}
{% include section.html %}
## Alumni
{% include list.html data="members" component="portrait" filter="group == 'alum'" %}
{% include section.html %}
## Join us!
{% include grid.html style="square" content=content %}
