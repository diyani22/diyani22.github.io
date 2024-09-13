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
    <!-- Video Slide 1 -->
    <div class="carousel-item">
      <iframe width="560" height="315" src="https://www.youtube.com/embed/cxliGPElThw?si=Z0FCxtVOaaKsrkXm" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
    </div>

    <!-- Video Slide 2 -->
    <div class="carousel-item">
      <iframe width="560" height="315" src="https://www.youtube.com/embed/BIACLUSYOu8?si=Su3huc9_nBKD-aaY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
    </div>

    <!-- Video Slide 3 -->
    <div class="carousel-item">
      <iframe width="560" height="315" src="https://www.youtube.com/embed/q85MrldzMeA?si=xMH1UrhIjPpsHpry" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
    </div>

    <!-- Video Slide 4 -->
    <div class="carousel-item">
      <iframe width="560" height="315" src="https://www.youtube.com/embed/W_xAsLPFYwA?si=gry3uUgtci8i6Mcz" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
    </div>

    <!-- Video Slide 5 -->
    <div class="carousel-item">
      <iframe width="560" height="315" src="https://www.youtube.com/embed/xbFg0ewZRXo?si=z78joNUBRCB1nYF5" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
    </div>

    <!-- Video Slide 6 -->
    <div class="carousel-item">
      <iframe width="560" height="315" src="https://www.youtube.com/embed/1RxuMFGP3wc?si=apSb1qQFZezWiLjz" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
    </div>

    <!-- Video Slide 7 -->
    <div class="carousel-item">
      <iframe width="560" height="315" src="https://www.youtube.com/embed/e-iE1iB5cBc?si=ImHAoZzO8DJyplUE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
    </div>

    <!-- Video Slide 8 -->
    <div class="carousel-item">
      <iframe width="560" height="315" src="https://www.youtube.com/embed/sJnUoWspX48?si=jq3pIJG2uTXAm1rx" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
    </div>

    <!-- Video Slide 9 -->
    <div class="carousel-item">
      <iframe width="560" height="315" src="https://www.youtube.com/embed/sKPD358dIxM?si=WsL8FF2A_uRzGWMz" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
    </div>

    <!-- Video Slide 10 -->
    <div class="carousel-item">
      <iframe width="560" height="315" src="https://www.youtube.com/embed/cHY696rrYbA?si=-vVEb9lWFJARg1LM" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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
  const itemsToShow = 4; // Number of items to show at a time
  let currentIndex = 0;

  function updateCarousel() {
    const offset = -currentIndex * (100 / itemsToShow);
    wrapper.style.transform = `translateX(${offset}%)`;
    // Disable arrows if at the ends
    document.querySelector('.carousel-arrow.left').disabled = currentIndex === 0;
    document.querySelector('.carousel-arrow.right').disabled = currentIndex >= items.length - itemsToShow;
  }

  function nextSlide() {
    if (currentIndex < items.length - itemsToShow) {
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

  // Initial setup
  updateCarousel();
</script>

<style>
  .carousel-container {
    width: 90%;
    max-width: 1200px;
    position: relative;
    overflow: hidden;
    margin: auto;
  }

  .carousel-wrapper {
    display: flex;
    transition: transform 0.5s ease-in-out;
  }

  .carousel-item {
    flex: 1 0 25%; /* Adjust percentage to show 3, 4, 5 videos at a time */
    box-sizing: border-box;
    padding: 0 10px; /* Space between videos */
  }

  .carousel-item iframe {
    width: 100%;
    height: 250px; /* Adjust as needed */
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

  .carousel-arrow:disabled {
    opacity: 0.5;
    cursor: not-allowed;
  }
</style>
