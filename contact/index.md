---
title: Contact
nav:
  order: 5
  tooltip: Email, address, and location
---

# {% include icon.html icon="fa-regular fa-envelope" %}Contact

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis
nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.

{%
  include button.html
  type="email"
  text="jiwang@unmc.edu"
  link="jiwang@unmc.edu"
%}
{%
  include button.html
  type="phone"
  text="(402)559-5100"
  link="+1-402-559-5100"
%}
{%
  include button.html
  type="address"
  tooltip="Our location on Google Maps for easy navigation"
  link="https://www.google.com/maps/place/Durham+Research+Center+II/@41.2555807,-95.9808617,16z/data=!4m15!1m8!3m7!1s0x87938e782fb074db:0xbe2fb8a5e591fab4!2sDurham+Research+Center+1,+S+45th+St,+Omaha,+NE+68131!3b1!8m2!3d41.2555807!4d-95.9808617!16s%2Fg%2F11_s0l5bl!3m5!1s0x87938e784ab1bc8b:0xf629a43420af9bf2!8m2!3d41.2548634!4d-95.9811769!16s%2Fg%2F11c5_1v4y_?entry=ttu&g_ep=EgoyMDI1MDExMC4wIKXMDSoASAFQAw%3D%3D"
%}

{% include section.html %}

{% capture col1 %}

{%
  include figure.html
  image="images/photo.jpg"
  caption="Lorem ipsum"
%}

{% endcapture %}

{% capture col2 %}

{%
  include figure.html
  image="images/photo.jpg"
  caption="Lorem ipsum"
%}

{% endcapture %}

{% include cols.html col1=col1 col2=col2 %}

{% include section.html dark=true %}

{% capture col1 %}
Lorem ipsum dolor sit amet  
consectetur adipiscing elit  
sed do eiusmod tempor
{% endcapture %}

{% capture col2 %}
Lorem ipsum dolor sit amet  
consectetur adipiscing elit  
sed do eiusmod tempor
{% endcapture %}

{% capture col3 %}
Lorem ipsum dolor sit amet  
consectetur adipiscing elit  
sed do eiusmod tempor
{% endcapture %}

{% include cols.html col1=col1 col2=col2 col3=col3 %}
