---
layout: page
title: Resources
permalink: /resources/
main_nav: true
---

<h1>Videos</h1>
<p>Below you will find videos covering the content of GCSE Computer Science to help you with your revision. Check them all out on my YouTube channel! - https://www.youtube.com/@compscicorner22</p>

# Video Carousel

<div class="carousel-container">
  <!-- Carousel wrapper holding multiple items -->
  <div class="carousel-wrapper">
    <!-- First Video Slide -->
    <div class="carousel-item">
      <iframe width="560" height="315" src="https://www.youtube.com/embed/cxliGPElThw?si=eCTbAHvD4h_PPZrw" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
    </div>

    <!-- Second Video Slide -->
    <div class="carousel-item">
      <iframe src="https://www.youtube.com/watch?v=BIACLUSYOu8&t=113s" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </div>

    <!-- Third Video Slide -->
    <div class="carousel-item">
      <iframe src="https://www.youtube.com/watch?v=q85MrldzMeA" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </div>

    <!-- Fourth Video Slide -->
    <div class="carousel-item">
      <iframe src="https://www.youtube.com/watch?v=W_xAsLPFYwA&t=2s" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </div>

    <!-- Fifth Video Slide -->
    <div class="carousel-item">
      <iframe src="https://www.youtube.com/watch?v=xbFg0ewZRXo" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </div>

    <!-- Sixth Video Slide -->
    <div class="carousel-item">
      <iframe width="560" height="315" src="https://www.youtube.com/embed/1RxuMFGP3wc?si=UIax7C9iWPiC-gd6" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
    </div>
  </div>

  <!-- Left Arrow -->
  <button class="carousel-arrow left" onclick="prevSlide()">&#10094;</button>

  <!-- Right Arrow -->
  <button class="carousel-arrow right" onclick="nextSlide()">&#10095;</button>
</div>

<script>
  const wrapper = document.querySelector('.carousel-wrapper');
  const items = document.querySelectorAll('.carousel-item');
  let currentIndex = 0;

  function updateCarousel() {
    const offset = -currentIndex * 100;
    wrapper.style.transform = `translateX(${offset}%)`;
  }

  function nextSlide() {
    if (currentIndex < items.length - 1) {
      currentIndex++;
      updateCarousel();
    }
  }

  function prevSlide() {
    if (currentIndex > 0) {
      currentIndex--;
      updateCarousel();
    }
  }
</script>

<style>
  .carousel-container {
    width: 80%;
    max-width: 800px;
    margin: 20px auto;
    position: relative;
    overflow: hidden;
  }

  .carousel-wrapper {
    display: flex;
    transition: transform 0.5s ease-in-out;
  }

  .carousel-item {
    min-width: 100%;
    box-sizing: border-box;
  }

  .carousel-item iframe {
    width: 100%;
    height: 450px;
  }

  .carousel-arrow {
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
    font-size: 2rem;
    color: #333;
    background-color: rgba(255, 255, 255, 0.7);
    border: none;
    padding: 0.5rem 1rem;
    cursor: pointer;
    z-index: 10;
  }

  .carousel-arrow.left {
    left: 10px;
  }

  .carousel-arrow.right {
    right: 10px;
  }
</style>

