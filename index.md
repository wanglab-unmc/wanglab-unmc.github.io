---
title: Home
nav:
  order: 1
  tooltip: Wang Lab @ UNMC
---

# Wang Lab

Dr. Wang's laboratory focuses on the intersection of machine learning and medical imaging. The lab develops and applies methods in machine learning, artificial intelligence, and data science to process and analyze medical images to understand the mechanisms of diseases and build diagnostic/predictive models.

## Highlights
<!-- Bootstrap 5 Image Slider -->
<div id="imageCarousel" class="carousel slide" data-bs-ride="carousel" style="width: 1000px; height: 450px; margin: auto; position: relative;">
  <!-- Indicators -->
  <div class="carousel-indicators">
    <button type="button" data-bs-target="#imageCarousel" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
    <button type="button" data-bs-target="#imageCarousel" data-bs-slide-to="1" aria-label="Slide 2"></button>
    <button type="button" data-bs-target="#imageCarousel" data-bs-slide-to="2" aria-label="Slide 3"></button>
    <button type="button" data-bs-target="#imageCarousel" data-bs-slide-to="3" aria-label="Slide 4"></button>
    <button type="button" data-bs-target="#imageCarousel" data-bs-slide-to="4" aria-label="Slide 5"></button>
  </div>

  <div class="carousel-inner">
    <div class="carousel-item active">
      <img src="images/cocaine.png" class="d-block w-100" style="height: 400px; object-fit: contain;" alt="Image 1">
      <div class="description">
        <h5>Functional Connectivity Alternation Analysis</h5>
      </div>
    </div>
    <div class="carousel-item">
      <img src="images/elae042f1.jpg" class="d-block w-100" style="height: 400px; object-fit: contain;" alt="Image 2">
      <div class="description">
        <h5>Brain Age Prediction Pipeline</h5>
      </div>
    </div>
    <div class="carousel-item">
      <img src="images/prostate_cancer.png" class="d-block w-100" style="height: 400px; object-fit: contain;" alt="Image 3">
      <div class="description">
        <h5>Predict overall survival in patients with metastatic prostate cancer</h5>
      </div>
    </div>
    <div class="carousel-item">
      <img src="images/ad.jpg" class="d-block w-100" style="height: 400px; object-fit: contain;" alt="Image 4">
      <div class="description">
        <h5>Pipeline of Alzheimer’s Disease Diagnosis</h5>
      </div>
    </div>
    <div class="carousel-item">
      <img src="images/lgn.jpg" class="d-block w-100" style="height: 400px; object-fit: contain;" alt="Image 5">
      <div class="description">
        <h5>Pipeline flow chart of automatic LGN segmentation</h5>
      </div>
    </div>
  </div>

  <!-- Controls -->
  <button class="carousel-control-prev custom-btn" type="button" data-bs-target="#imageCarousel" data-bs-slide="prev">
    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Previous</span>
  </button>
  
  <button class="carousel-control-next custom-btn" type="button" data-bs-target="#imageCarousel" data-bs-slide="next">
    <span class="carousel-control-next-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Next</span>
  </button>
</div>

<style>
  /* Description Styling */
  .description {
    text-align: center;
    padding: 10px;
    background: rgba(0, 0, 0, 0.1); /* Light background to differentiate */
    color: black;
    font-size: 18px;
  }

  /* Custom Navigation Buttons */
  .custom-btn {
    width: 60px; /* Make the buttons larger */
    height: 60px;
    background-color: rgba(0, 0, 0, 0.5); /* Darker background for visibility */
    border-radius: 50%; /* Circular buttons */
  }

  .custom-btn:hover {
    background-color: rgba(0, 0, 0, 0.8); /* Darker hover effect */
  }

  .carousel-control-prev-icon,
  .carousel-control-next-icon {
    width: 50px; /* Larger icons */
    height: 50px;
  }
</style>

{% include section.html %}
## Latest News

{% assign latest_news = site.data.news | sort: "date" | reverse | slice: 0, 5 %}

<div class="latest-news">
  <ul class="news-list">
    {% for news in latest_news %}
      <li>
        <span class="news-date">{{ news.date | date: "<b>%b %d, %Y</b>" }}</span>: {{ news.title }}
      </li>
    {% endfor %}
  </ul>

  <div class="news-load-more">
    <a href="{{ '/news/' | relative_url }}" class="button">Load More</a>
  </div>
</div>
