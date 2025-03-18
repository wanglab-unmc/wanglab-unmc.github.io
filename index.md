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
<div id="imageCarousel" class="carousel slide" data-bs-ride="carousel" style="width: 1000px; height: 600px; margin: auto; position: relative;">
  <!-- Indicators -->
  <div class="carousel-indicators">
    <button type="button" data-bs-target="#imageCarousel" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
    <button type="button" data-bs-target="#imageCarousel" data-bs-slide-to="1" aria-label="Slide 2"></button>
    <button type="button" data-bs-target="#imageCarousel" data-bs-slide-to="2" aria-label="Slide 3"></button>
  </div>

  <div class="carousel-inner">
    <div class="carousel-item active">
      <div class="carousel-caption d-block text-dark" style="{% raw %}position: absolute; top: 10px; left: 50%; transform: translateX(-50%); background: rgba(255, 255, 255, 0.7); padding: 10px; border-radius: 5px;{% endraw %}">
        <h5>Description for Image 1</h5>
      </div>
      <img src="images/cocaine_fig1.png" class="d-block w-100" style="height: 600px; object-fit: contain;" alt="Image 1">
    </div>
    <div class="carousel-item">
      <div class="carousel-caption d-block text-dark" style="{% raw %}position: absolute; top: 10px; left: 50%; transform: translateX(-50%); background: rgba(255, 255, 255, 0.7); padding: 10px; border-radius: 5px;{% endraw %}">
        <h5>Description for Image 2</h5>
      </div>
      <img src="images/elae042f1.jpg" class="d-block w-100" style="height: 600px; object-fit: contain;" alt="Image 2">
    </div>
    <div class="carousel-item">
      <div class="carousel-caption d-block text-dark" style="{% raw %}position: absolute; top: 10px; left: 50%; transform: translateX(-50%); background: rgba(255, 255, 255, 0.7); padding: 10px; border-radius: 5px;{% endraw %}">
        <h5>Description for Image 3</h5>
      </div>
      <img src="images/cocaine_fig2.png" class="d-block w-100" style="height: 600px; object-fit: contain;" alt="Image 3">
    </div>
  </div>

  <!-- Controls -->
  <button class="carousel-control-prev" type="button" data-bs-target="#imageCarousel" data-bs-slide="prev">
    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Previous</span>
  </button>
  <button class="carousel-control-next" type="button" data-bs-target="#imageCarousel" data-bs-slide="next">
    <span class="carousel-control-next-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Next</span>
  </button>
</div>


{% include section.html %}
## Latest News

{% assign latest_news = site.data.news | sort: "date" | reverse | slice: 0, 5 %}

<div class="latest-news">
  <ul class="news-list">
    {% for news in latest_news %}
      <li>
        <span class="news-date">{{ news.date | date: "%d %b, %Y" }}</span>: {{ news.title }}
      </li>
    {% endfor %}
  </ul>

  <div class="news-load-more">
    <a href="{{ '/news/' | relative_url }}" class="button">Load More</a>
  </div>
</div>
