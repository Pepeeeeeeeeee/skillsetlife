<script setup>
import { onMounted } from 'vue';
let slides;
let dots;
let slideIndex = 1;

onMounted(() => {
  slides = document.getElementsByClassName("slide");
  dots = document.getElementsByClassName("dot");
  console.log(slides);
  showSlides(slideIndex);
});


// Next/previous controls
function plusSlides(n) {
  showSlides(slideIndex += n);
}

// Thumbnail image controls
function currentSlide(n) {
  showSlides(slideIndex = n);
}

function showSlides(n) {
  let i;
  if (n > slides.length) {slideIndex = 1}
  if (n < 1) {slideIndex = slides.length}
  for (i = 0; i < slides.length; i++) {
    slides[i].style.display = "none";
  }
  for (i = 0; i < dots.length; i++) {
    dots[i].className = dots[i].className.replace(" active", "");
  }
  slides[slideIndex-1].style.display = "block";
  dots[slideIndex-1].className += " active";
}
</script>

<template>
<div class="testimonials-container">
  <div class="slide fade">
    <div class="statement s-right">
      <div class="testemony">
        <p class="statement-text">"Lorem ipsum, dolor sit amet consectetur adipisicing elit."</p>
        <p class="rating">10/10</p>
      </div>
      <div class="customer">
        <img class="customer-photo" src="../assets/user-2935527.svg" alt="">
        <p class="customer-desc">Lorem, ipsum dolor.</p>
      </div>
    </div>
    <div class="statement s-left">
      <div class="customer">
        <img class="customer-photo" src="../assets/user-2935527.svg" alt="">
        <p class="customer-desc">Lorem, ipsum dolor.</p>
      </div>
      <div class="testemony">
        <p class="statement-text">"Lorem ipsum, dolor sit amet consectetur adipisicing elit."</p>
        <p class="rating">10/10</p>
      </div>
    </div>
  </div>

  <div class="slide fade">
    <div class="statement s-left">
      <div class="customer">
        <img class="customer-photo" src="../assets/user-2935527.svg" alt="">
        <p class="customer-desc">Lorem, ipsum dolor.</p>
      </div>
      <div class="testemony">
        <p class="statement-text">"Lorem ipsum, dolor sit amet consectetur adipisicing elit."</p>
        <p class="rating">10/10</p>
      </div>
    </div>
    <div class="statement s-right">
      <div class="testemony">
        <p class="statement-text">"Lorem ipsum, dolor sit amet consectetur adipisicing elit."</p>
        <p class="rating">10/10</p>
      </div>
      <div class="customer">
        <img class="customer-photo" src="../assets/user-2935527.svg" alt="">
        <p class="customer-desc">Lorem, ipsum dolor.</p>
      </div>
    </div>
  </div>

  <div class="slide fade">
    <div class="statement s-right">
      <div class="testemony">
        <p class="statement-text">"Lorem ipsum, dolor sit amet consectetur adipisicing elit."</p>
        <p class="rating">10/10</p>
      </div>
      <div class="customer">
        <img class="customer-photo" src="../assets/user-2935527.svg" alt="">
        <p class="customer-desc">Lorem, ipsum dolor.</p>
      </div>
    </div>
    <div class="statement s-left">
      <div class="customer">
        <img class="customer-photo" src="../assets/user-2935527.svg" alt="">
        <p class="customer-desc">Lorem, ipsum dolor.</p>
      </div>
      <div class="testemony">
        <p class="statement-text">"Lorem ipsum, dolor sit amet consectetur adipisicing elit."</p>
        <p class="rating">10/10</p>
      </div>
    </div>
  </div>

  <div class="slide fade">
    <div class="statement s-left">
      <div class="customer">
        <img class="customer-photo" src="../assets/user-2935527.svg" alt="">
        <p class="customer-desc">Lorem, ipsum dolor.</p>
      </div>
      <div class="testemony">
        <p class="statement-text">"Lorem ipsum, dolor sit amet consectetur adipisicing elit."</p>
        <p class="rating">10/10</p>
      </div>
    </div>
    <div class="statement s-right">
      <div class="testemony">
        <p class="statement-text">"Lorem ipsum, dolor sit amet consectetur adipisicing elit."</p>
        <p class="rating">10/10</p>
      </div>
      <div class="customer">
        <img class="customer-photo" src="../assets/user-2935527.svg" alt="">
        <p class="customer-desc">Lorem, ipsum dolor.</p>
      </div>
    </div>
  </div>

  <div class="slide fade">
    <div class="statement s-right">
      <div class="testemony">
        <p class="statement-text">"Lorem ipsum, dolor sit amet consectetur adipisicing elit."</p>
        <p class="rating">10/10</p>
      </div>
      <div class="customer">
        <img class="customer-photo" src="../assets/user-2935527.svg" alt="">
        <p class="customer-desc">Lorem, ipsum dolor.</p>
      </div>
    </div>
    <div class="statement s-left">
      <div class="customer">
        <img class="customer-photo" src="../assets/user-2935527.svg" alt="">
        <p class="customer-desc">Lorem, ipsum dolor.</p>
      </div>
      <div class="testemony">
        <p class="statement-text">"Lorem ipsum, dolor sit amet consectetur adipisicing elit."</p>
        <p class="rating">10/10</p>
      </div>
    </div>
  </div>


  <!-- Next and previous buttons -->
  <a class="prev" @click="plusSlides(-1)">&#10094;</a>
  <a class="next" @click="plusSlides(1)">&#10095;</a>
</div>
<br>

<!-- The dots/circles -->
<div style="text-align:center">
<span class="dot" @click="currentSlide(1)"></span>
<span class="dot" @click="currentSlide(2)"></span>
<span class="dot" @click="currentSlide(3)"></span>
<span class="dot" @click="currentSlide(4)"></span>
<span class="dot" @click="currentSlide(5)"></span>
</div>
</template>

<style scoped>
* {box-sizing:border-box}

/* Slideshow container */
.testimonials-container {
  max-width: 1000px;
  position: relative;
  margin: auto;
}

/* Hide the images by default */
.slide {
  display: none;
  width: 50%;
  margin: auto;
}

.statement {
  display: flex;
  position: relative;
  gap: 2em;
  margin: 25px 0;
}

.statement.s-right {
  text-align: right;
  right: -75px;
}

.statement.s-left {
  left: -75px;
}

.testemony {
  margin:auto;
}

.rating {
  font-size: larger;
}

.customer-desc {
  text-align: center;
}

.customer-photo {
  width: 128px;
  border-radius: 25%;
} 

/* Next & previous buttons */
.prev, .next {
  cursor: pointer;
  position: absolute;
  top: 50%;
  width: auto;
  margin-top: -22px;
  padding: 16px;
  color: #2395E7;
  font-weight: bold;
  font-size: 18px;
  transition: 0.6s ease;
  border-radius: 3px;
  user-select: none;
}

/* Position the "next button" to the right */
.next {
  right: 0;
}

.prev {
  left: 0;
}

/* On hover, add a black background color with a little bit see-through */
.prev:hover, .next:hover {
  background-color: rgba(0,0,0,0.8);
}

/* Caption text */
.text {
  color: #f2f2f2;
  font-size: 15px;
  padding: 8px 12px;
  position: absolute;
  bottom: 8px;
  width: 100%;
  text-align: center;
}

/* Number text (1/3 etc) */
.numbertext {
  color: #f2f2f2;
  font-size: 12px;
  padding: 8px 12px;
  position: absolute;
  top: 0;
}

/* The dots/bullets/indicators */
.dot {
  cursor: pointer;
  height: 15px;
  width: 15px;
  margin: 0 2px;
  background-color: #bbb;
  border-radius: 50%;
  display: inline-block;
  transition: background-color 0.6s ease;
}

.active, .dot:hover {
  background-color: #717171;
}

/* Fading animation */
.fade {
  animation-name: fade;
  animation-duration: 1.5s;
}

@keyframes fade {
  from {opacity: .4}
  to {opacity: 1}
}
</style>
