---
title: Home
nav:
  order: 1
  tooltip: Wang Lab @ UNMC
---

# Wang Lab

Dr. Wang's laboratory focuses on the intersection of machine learning and medical imaging. The lab develops and applies methods in machine learning, artificial intelligence, and data science to process and analyze medical images to understand the mechanisms of diseases and build diagnostic/predictive models.

## Highlights
<div id="imageCarousel" class="carousel slide" data-bs-ride="carousel" style="width: 1000px; height: 600px; margin: auto;">
  <div class="carousel-inner">
    <div class="carousel-item active">
      <img src="images/cocaine_fig1.png" class="d-block w-100" style="height: 600px; object-fit: cover;" alt="Image 1">
    </div>
    <div class="carousel-item">
      <img src="images/elae042f1.jpg" class="d-block w-100" style="height: 600px; object-fit: cover;" alt="Image 2">
    </div>
    <div class="carousel-item">
      <img src="images/cocaine_fig2.png" class="d-block w-100" style="height: 600px; object-fit: cover;" alt="Image 3">
    </div>
  </div>
</div>

{% include section.html %}
## Latest News

{% assign latest_news = site.data.news | sort: "date" | reverse | slice: 0, 5 %}

{% for news in latest_news %}
<div class="news">
  {% if news.image %}
    <a href="{{ news.link | relative_url | uri_escape }}" class="news-image">
      <img src="{{ news.image | relative_url | uri_escape }}" alt="{{ news.title }}">
    </a>
  {% endif %}

  <div class="news-text">
    <a href="{{ news.link | relative_url | uri_escape }}" class="news-title">
      {{ news.title }}
    </a>

    <div class="news-details">
      <span class="news-date">{{ news.date | date: "%b %d, %Y" }}</span>
    </div>

    {% if news.description %}
      <div class="news-description">
        {{ news.description | markdownify | remove: "<p>" | remove: "</p>" }}
      </div>
    {% endif %}
  </div>
</div>
{% endfor %}

