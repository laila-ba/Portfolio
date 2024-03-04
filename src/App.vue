import Home from './views/Home.vue';

<template>
  <body class="bg-gray-900">
    <router-view>hello1</router-view>
    <!-- <canvas id="hero-lightpass" /> -->
  </body>
</template>

<style>
@import url("https://fonts.cdnfonts.com/css/mark-pro?styles=78514");
@import url("https://fonts.cdnfonts.com/css/circular-std?styles=17909");

#app {
  font-family: "circular std", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

a {
  font-family: "Mark Pro";
}
h1,
h2 {
  font-family: "Mark Pro";
}
@-webkit-keyframes gradient {
  0% {
    background-position: 0 50%;
  }

  50% {
    background-position: 100% 50%;
  }

  to {
    background-position: 0 50%;
  }
}

@keyframes gradient {
  0% {
    background-position: 0 50%;
  }

  50% {
    background-position: 100% 50%;
  }

  to {
    background-position: 0 50%;
  }
}

@-webkit-keyframes logoLeftAnim {
  0% {
    -webkit-transform: translateX(0);
    transform: translateX(0);
  }

  20% {
    -webkit-transform: translate(-110%);
    transform: translate(-110%);
  }

  50%,
  to {
    -webkit-transform: translate(0);
    transform: translate(0);
  }
}

@keyframes logoLeftAnim {
  0% {
    -webkit-transform: translateX(0);
    transform: translateX(0);
  }

  20% {
    -webkit-transform: translate(-110%);
    transform: translate(-110%);
  }

  50%,
  to {
    -webkit-transform: translate(0);
    transform: translate(0);
  }
}

@-webkit-keyframes reviewCardAnim1 {
  0% {
    -webkit-transform: translateX(-52%);
    transform: translateX(-52%);
  }

  to {
    -webkit-transform: translateX(0);
    transform: translateX(0);
  }
}

@keyframes reviewCardAnim1 {
  0% {
    -webkit-transform: translateX(-52%);
    transform: translateX(-52%);
  }

  to {
    -webkit-transform: translateX(0);
    transform: translateX(0);
  }
}

@-webkit-keyframes reviewCardAnim2 {
  0% {
    -webkit-transform: translateX(0);
    transform: translateX(0);
  }

  to {
    -webkit-transform: translateX(-52%);
    transform: translateX(-52%);
  }
}

@keyframes reviewCardAnim2 {
  0% {
    -webkit-transform: translateX(0);
    transform: translateX(0);
  }

  to {
    -webkit-transform: translateX(-52%);
    transform: translateX(-52%);
  }
}

@-webkit-keyframes rect1Anim {
  0% {
    height: 5.8px;
  }

  50% {
    height: 8px;
  }

  to {
    height: 1px;
  }
}

@keyframes rect1Anim {
  0% {
    height: 5.8px;
  }

  50% {
    height: 8px;
  }

  to {
    height: 1px;
  }
}

@-webkit-keyframes rect2Anim {
  0% {
    height: 5.8px;
  }

  50% {
    height: 6px;
  }

  to {
    height: 4px;
  }
}

@keyframes rect2Anim {
  0% {
    height: 5.8px;
  }

  50% {
    height: 6px;
  }

  to {
    height: 4px;
  }
}

@-webkit-keyframes rect3Anim {
  0% {
    height: 5.8px;
  }

  50% {
    height: 4px;
  }

  to {
    height: 8px;
  }
}

@keyframes rect3Anim {
  0% {
    height: 5.8px;
  }

  50% {
    height: 4px;
  }

  to {
    height: 8px;
  }
}

@-webkit-keyframes rect4Anim {
  0% {
    height: 5.8px;
  }

  50% {
    height: 1px;
  }

  to {
    height: 3px;
  }
}

@keyframes rect4Anim {
  0% {
    height: 5.8px;
  }

  50% {
    height: 1px;
  }

  to {
    height: 3px;
  }
}

@-webkit-keyframes cursorAnim {
  0% {
    -webkit-transform: rotate(0deg);
    transform: rotate(0deg);
  }

  to {
    -webkit-transform: rotate(1turn);
    transform: rotate(1turn);
  }
}

@keyframes cursorAnim {
  0% {
    -webkit-transform: rotate(0deg);
    transform: rotate(0deg);
  }

  to {
    -webkit-transform: rotate(1turn);
    transform: rotate(1turn);
  }
}

.rot {
  -webkit-animation: cursorAnim 1s linear infinite;
  animation: cursorAnim 1s linear infinite;
}

@-webkit-keyframes preloaderTextAnim {
  0% {
    -webkit-transform: translateY(0);
    transform: translateY(0);
  }

  50%,
  to {
    -webkit-transform: translateY(-600%);
    transform: translateY(-600%);
  }
}

@keyframes preloaderTextAnim {
  0% {
    -webkit-transform: translateY(0);
    transform: translateY(0);
  }

  50%,
  to {
    -webkit-transform: translateY(-600%);
    transform: translateY(-600%);
  }
}

:root {
  --color-white: #fff;
  --color-gray: #c4c4c4;
  --color-black: #000;
  --color-purple: #8000ff;
  --color-light-purple: #cf59e6;
  --color-light-blue: #6bc5f8;
}

.about {
  grid-column: 2/14;
  margin-top: 20rem;
  padding: 0 6rem;
}

@media only screen and (max-width: 57em) {
  .about {
    grid-column: 1/15;
  }
}

@media only screen and (max-width: 45em) {
  .about {
    padding: 0 4rem;
  }
}

.about .about-card {
  width: 70%;
  margin: 20rem auto;
  background: -webkit-gradient(
    linear,
    left top,
    left bottom,
    from(rgba(35, 37, 49, 0.5)),
    to(rgb(17 24 39))
  );
  background: -webkit-linear-gradient(
    top,
    rgba(35, 37, 49, 0.5),
    rgba(15, 15, 24, 0.5)
  );
  background: linear-gradient(
    180deg,
    rgba(35, 37, 49, 0.5),
    rgba(15, 15, 24, 0.5)
  );
  border: 0.2rem solid #20222e;
  -webkit-box-sizing: border-box;
  box-sizing: border-box;
  -webkit-backdrop-filter: blur(54px);
  backdrop-filter: blur(54px);
  border-radius: 7.3rem;
  display: flex;
  align-items: center;
  padding: 6rem;
  position: relative;
}

@media only screen and (max-width: 57em) {
  .about .about-card {
    width: 70%;
    border-radius: 6.3rem;
    flex-direction: column;
  }
}

@media only screen and (max-width: 40em) {
  .about .about-card {
    width: 75%;
  }
}

@media only screen and (max-width: 35em) {
  .about .about-card {
    width: 80%;
  }
}

@media only screen and (max-width: 30em) {
  .about .about-card {
    padding: 4rem;
    width: 84%;
    border-radius: 4.3rem;
  }
}

@media only screen and (max-width: 23em) {
  .about .about-card {
    width: 90%;
  }
}

@media only screen and (max-width: 22em) {
  .about .about-card {
    width: 100%;
  }
}

.about .about-card:before {
  content: "";
  display: block;
  position: absolute;
  top: -5rem;
  right: -5rem;
  width: 15rem;
  height: 15rem;
  background-repeat: no-repeat;
  background-size: contain;
}

@media only screen and (max-width: 57em) {
  .about .about-card:before {
    top: -3rem;
    right: -3rem;
    width: 12rem;
    height: 12rem;
  }
}

.about .about-card:first-of-type:before {
  background-image: url(/src\assets\img\01.png);
}

.about.about-card__left {
  margin-right: 6rem;
}

@media only screen and (max-width: 57em) {
  .about .about-card__left {
    order: 2;
    display: flex;
    align-self: flex-start;
    display: none;
  }
}

.about .about-card__left h4 {
  -webkit-transform: rotate(180deg);
  transform: rotate(180deg);
  -webkit-writing-mode: tb-rl;
  -ms-writing-mode: tb-rl;
  writing-mode: tb-rl;
  font-family: D-DIN Condensed, sans-serif;
  font-size: 1.3rem;
  line-height: 92.4%;
  letter-spacing: 0.19em;
  color: #8b8b8b;
  line-height: 120%;
}

@media only screen and (max-width: 57em) {
  .about .about-card__left h4 {
    -webkit-transform: rotate(1turn);
    transform: rotate(1turn);
    -webkit-writing-mode: lr-tb;
    -ms-writing-mode: lr-tb;
    writing-mode: lr-tb;
    margin-top: 3rem;
    margin-bottom: 2rem;
  }
}

.about .about-card__middle {
  width: 35rem;
  height: 45rem;
  background-size: cover;
  position: relative;
  border-radius: 5.3rem;
  overflow: hidden;
}

@media only screen and (max-width: 57em) {
  .about .about-card__middle {
    order: 1;
    border-radius: 5rem;
    height: 40rem;
  }
}

@media only screen and (max-width: 30em) {
  .about .about-card__middle {
    width: 30rem;
    border-radius: 3rem;
  }
}

.about .about-card__middle canvas {
  position: absolute;
  z-index: 0;
  width: 100% !important;
  height: 100% !important;
}

.about .about-card__middle img {
  width: 100%;
  height: 100%;
}

.about .about-card__middle img:hover:nth-child(2) {
  opacity: 1;
}

.about .about-card__middle img:first-child,
.about .about-card__middle img:nth-child(2) {
  position: absolute;
  top: 0;
  left: 0;
  opacity: 0;
  -webkit-transition: opacity 0.3s;
  transition: opacity 0.3s;
}

.about .about-card__right {
  margin-left: 6rem;
}

@media only screen and (max-width: 57em) {
  .about .about-card__right {
    margin-left: 0;
    display: flex;
    flex-direction: column;
    align-self: flex-start;
    order: 3;
    margin-top: 2rem;
  }
}

.about .about-card__right h2 {
  margin-bottom: 6rem;
}

@media only screen and (max-width: 57em) {
  .about .about-card__right h2 {
    margin-bottom: 3rem;
  }
}

.about .about-card__link {
  display: inline-block;
  font-family: D-DIN Condensed, sans-serif;
  font-size: 1.8rem;
  line-height: 92.4%;
  letter-spacing: 0.19em;
  text-decoration: none;
  position: relative;
}

.about .about-card__link:after {
  display: block;
  content: "";
  position: absolute;
  bottom: -1rem;
  left: 0;
  width: 50%;
  height: 1px;
  background: var(--color-gray);
  -webkit-transition: all 0.3s ease;
  transition: all 0.3s ease;
}

.about .about-card__link:hover:after {
  width: 100%;
}

*,
:after,
:before {
  margin: 0;
  padding: 0;
  -webkit-box-sizing: inherit;
  box-sizing: inherit;
}

html {
  height: 100vh;
  -webkit-box-sizing: border-box;
  box-sizing: border-box;
  text-rendering: optimizeLegibility;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  scroll-behavior: smooth;
}

body {
  overflow-x: hidden;
}

.cursor {
  width: 8rem;
  height: 8rem;
  position: absolute;
  top: 40%;
  right: 20%;
  pointer-events: none;
  -webkit-transition: left top 0.1s ease-in-out;
  transition: left top 0.1s ease-in-out;
  z-index: 1233333;
  background-image: url(/_next/static/media/cursor.15b239677e06a3d70edb0bb22c673add.svg);
  background-size: contain;
  background-repeat: no-repeat;
  -webkit-animation: cursorAnim 10s linear infinite;
  animation: cursorAnim 10s linear infinite;
}

@media only screen and (max-width: 52.5em) {
  .cursor {
    opacity: 0;
  }
}

.reveal {
  position: relative;
  transform: translateY(150px);
  opacity: 0;
  transition: 1s all ease;
}

.reveal.active {
  transform: translateY(0);
  opacity: 1;
}
</style>

<script>
function reveal() {
  var reveals = document.querySelectorAll(".reveal");

  for (var i = 0; i < reveals.length; i++) {
    var windowHeight = window.innerHeight;
    var elementTop = reveals[i].getBoundingClientRect().top;
    var elementVisible = 150;

    if (elementTop < windowHeight - elementVisible) {
      reveals[i].classList.add("active");
    } else {
      reveals[i].classList.remove("active");
    }
  }
}

window.addEventListener("scroll", reveal);

export default {};
</script>
