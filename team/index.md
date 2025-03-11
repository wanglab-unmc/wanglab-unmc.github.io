---
title: Team
nav:
  order: 4
  tooltip: About our team
---

# {% include icon.html icon="fa-solid fa-users" %}Team
## Principal Investigator
{% include list.html data="members" component="portrait" filter="role == 'pi'" %}
## Postdoctoral Researchers
{% include list.html data="members" component="portrait" filter="role == 'postdoc'" %}
## Students
{% include list.html data="members" component="portrait" filter="role == 'phd'" %}
## Research Technician
{% include list.html data="members" component="portrait" filter="role == 'tech'" %}
## Intern Students
{% include list.html data="members" component="portrait" filter="role == 'intern'" %}
{% include section.html %}
## Alumni
{% include list.html data="members" component="portrait" filter="group == 'alum'" %}
{% include section.html %}
## Join us!
