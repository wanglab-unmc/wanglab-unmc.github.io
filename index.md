---
title: Home
nav:
  order: 1
  tooltip: Wang Lab @ UNMC
---

# Wang Lab

Dr. Wang's laboratory focuses on the intersection of machine learning and medical imaging. The lab develops and applies methods in machine learning, artificial intelligence, and data science to process and analyze medical images to understand the mechanisms of diseases and build diagnostic/predictive models.

{% include section.html %}

## Highlights

<div id="imageCarousel" class="carousel slide" data-bs-ride="carousel">
  <div class="carousel-inner">
    <div class="carousel-item active">
      <img src="images/cocaine_fig1.png" class="d-block w-100" alt="Image 1">
    </div>
    <div class="carousel-item">
      <img src="images/photo.jpg" class="d-block w-100" alt="Image 2">
    </div>
    <div class="carousel-item">
      <img src="images/photo.jpg" class="d-block w-100" alt="Image 3">
    </div>
  </div>
</div>

{% capture text %}

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.

{%
  include button.html
  link="research"
  text="See our publication"
  icon="fa-solid fa-arrow-right"
  flip=true
  style="bare"
%}

{% endcapture %}

{%
  include feature.html
  image="images/photo.jpg"
  link="research"
  title="Our Publication"
  text=text
%}

{% capture text %}

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.

{%
  include button.html
  link="projects"
  text="Browse our research"
  icon="fa-solid fa-arrow-right"
  flip=true
  style="bare"
%}

{% endcapture %}

{%
  include feature.html
  image="images/photo.jpg"
  link="projects"
  title="Our Research"
  flip=true
  style="bare"
  text=text
%}

{% capture text %}

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.

{%
  include button.html
  link="team"
  text="Meet our team"
  icon="fa-solid fa-arrow-right"
  flip=true
  style="bare"
%}

{% endcapture %}

{%
  include feature.html
  image="images/photo.jpg"
  link="team"
  title="Our Team"
  text=text
%}
