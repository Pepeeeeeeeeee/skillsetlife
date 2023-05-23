<script setup>
import { onMounted } from 'vue';
let slides;
let dots;
let slideIndex = 1;

onMounted(() => {
  slides = document.getElementsByClassName("slide");
  dots = document.getElementsByClassName("dot");
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
  <div class="slides">
    <div class="slide fade">
      <div class="statement s-right">
        <div class="testemony">
          <p class="statement-text">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Doloremque magnam dolor perferendis possimus unde accusantium, nam, aliquid blanditiis itaque necessitatibus vitae dolore veritatis? Rerum?</p>
          <p class="rating">10/10</p>
        </div>
        <div class="customer">
          <img class="customer-photo" src="../assets/user-2935527.svg" alt="">
          <p class="customer-desc">Lorem, ipsum dolor.</p>
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
          <p class="statement-text">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Doloremque magnam dolor perferendis possimus unde accusantium, nam, aliquid blanditiis itaque necessitatibus vitae dolore veritatis? Rerum?</p>
          <p class="rating">10/10</p>
        </div>
      </div>
    </div>
  
    <div class="slide fade">
      <div class="statement s-right">
        <div class="testemony">
          <p class="statement-text">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Doloremque magnam dolor perferendis possimus unde accusantium, nam, aliquid blanditiis itaque necessitatibus vitae dolore veritatis? Rerum?</p>
          <p class="rating">10/10</p>
        </div>
        <div class="customer">
          <img class="customer-photo" src="../assets/user-2935527.svg" alt="">
          <p class="customer-desc">Lorem, ipsum dolor.</p>
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
          <p class="statement-text">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Doloremque magnam dolor perferendis possimus unde accusantium, nam, aliquid blanditiis itaque necessitatibus vitae dolore veritatis? Rerum?</p>
          <p class="rating">10/10</p>
        </div>
      </div>
    </div>
  
    <div class="slide fade">
      <div class="statement s-right">
        <div class="testemony">
          <p class="statement-text">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Doloremque magnam dolor perferendis possimus unde accusantium, nam, aliquid blanditiis itaque necessitatibus vitae dolore veritatis? Rerum?</p>
          <p class="rating">10/10</p>
        </div>
        <div class="customer">
          <img class="customer-photo" src="../assets/user-2935527.svg" alt="">
          <p class="customer-desc">Lorem, ipsum dolor.</p>
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
          <p class="statement-text">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Doloremque magnam dolor perferendis possimus unde accusantium, nam, aliquid blanditiis itaque necessitatibus vitae dolore veritatis? Rerum?</p>
          <p class="rating">10/10</p>
        </div>
      </div>
    </div>
  
    <div class="slide fade">
      <div class="statement s-right">
        <div class="testemony">
          <p class="statement-text">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Doloremque magnam dolor perferendis possimus unde accusantium, nam, aliquid blanditiis itaque necessitatibus vitae dolore veritatis? Rerum?</p>
          <p class="rating">10/10</p>
        </div>
        <div class="customer">
          <img class="customer-photo" src="../assets/user-2935527.svg" alt="">
          <p class="customer-desc">Lorem, ipsum dolor.</p>
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
          <p class="statement-text">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Doloremque magnam dolor perferendis possimus unde accusantium, nam, aliquid blanditiis itaque necessitatibus vitae dolore veritatis? Rerum?</p>
          <p class="rating">10/10</p>
        </div>
      </div>
    </div>
  
    <div class="slide fade">
      <div class="statement s-right">
        <div class="testemony">
          <p class="statement-text">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Doloremque magnam dolor perferendis possimus unde accusantium, nam, aliquid blanditiis itaque necessitatibus vitae dolore veritatis? Rerum?</p>
          <p class="rating">10/10</p>
        </div>
        <div class="customer">
          <img class="customer-photo" src="../assets/user-2935527.svg" alt="">
          <p class="customer-desc">Lorem, ipsum dolor.</p>
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
          <p class="statement-text">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Doloremque magnam dolor perferendis possimus unde accusantium, nam, aliquid blanditiis itaque necessitatibus vitae dolore veritatis? Rerum?</p>
          <p class="rating">10/10</p>
        </div>
      </div>
    </div>
  
    <!-- Next and previous buttons -->
    <a class="prev" @click="plusSlides(-1)">&#10094;</a>
    <a class="next" @click="plusSlides(1)">&#10095;</a>
  </div>
</div>
<br>

<!-- The dots/circles -->
<div style="text-align:center">
<span class="dot" @click="currentSlide(1)"></span>
<span class="dot" @click="currentSlide(2)"></span>
<span class="dot" @click="currentSlide(3)"></span>
<span class="dot" @click="currentSlide(4)"></span>
<span class="dot" @click="currentSlide(5)"></span>
<span class="dot" @click="currentSlide(6)"></span>
<span class="dot" @click="currentSlide(7)"></span>
<span class="dot" @click="currentSlide(8)"></span>
<span class="dot" @click="currentSlide(9)"></span>
<span class="dot" @click="currentSlide(10)"></span>
</div>
</template>

<style scoped>
* {box-sizing:border-box}

/* Slideshow container */
.testimonials-container{
  background-color: #2395E7;
  padding: 2em;
  color: white;
}


.slides {
  max-width: 1000px;
  position: relative;
  margin: auto;
}

/* Hide the images by default */
.slide {
  display: none;
  margin: auto;
}

.statement {
  display: flex;
  gap: 5em;
  margin: 25px 0;
}

.statement-text {
  font-weight: bolder;
  font-size: x-large;
  line-height: 2em;
}

.statement.s-right {
  text-align: right;
}

.statement.s-left {
  text-align: left;
}

.testemony {
  margin:auto;
}

.rating {
  font-size: xx-large;
}

.customer-desc {
  text-align: center;
}

.customer-photo {
  width: 265px;
  border-radius: 25%;
} 

/* Next & previous buttons */
.prev, .next {
  cursor: pointer;
  position: absolute;
  bottom: -15%;
  width: auto;
  padding: 16px;
  color: #ffffff;
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
