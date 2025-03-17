---
title: Contact
nav:
  order: 7
  tooltip: Email, address, and location
---

# {% include icon.html icon="fa-regular fa-envelope" %}Contact

{%
  include button.html
  type="email"
  text="jiwang@unmc.edu"
  link="jiwang@unmc.edu"
%}
{%
  include button.html
  type="phone"
  text="(402) 559-5100"
  link="+1-402-559-5100"
%}
{%
  include button.html
  type="address"
  tooltip="Our location on Google Maps for easy navigation"
  link="https://www.google.com/maps/place/Durham+Research+Center+II/@41.2548634,-95.9837518,16z/data=!3m1!4b1!4m6!3m5!1s0x87938e784ab1bc8b:0xf629a43420af9bf2!8m2!3d41.2548634!4d-95.9811769!16s%2Fg%2F11c5_1v4y_?entry=ttu&g_ep=EgoyMDI1MDExMC4wIKXMDSoASAFQAw%3D%3D"
%}

{% include section.html %}

{% capture col1 %}

{%
  include figure.html
  image="images/DRCII.jpg"
  caption="View of DRC II"
%}

{% endcapture %}

{% include cols.html col1=col1 %}
