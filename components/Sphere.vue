<template>
  <section>
    <div class="sphere">
      <img src="../assets/blue-ribbon.svg" alt="" />
    </div>
    <div class="circle">
      <span style="--i: 1">L</span>
      <span style="--i: 2">e</span>
      <span style="--i: 3"> </span>
      <span style="--i: 4">P</span>
      <span style="--i: 5">'</span>
      <span style="--i: 6">t</span>
      <span style="--i: 7">i</span>
      <span style="--i: 8">t</span>
      <span style="--i: 9"> </span>
      <span style="--i: 10">H</span>
      <span style="--i: 11">o</span>
      <span style="--i: 12">m</span>
      <span style="--i: 13">m</span>
      <span style="--i: 14">e</span>
      <span style="--i: 15"> </span>
      <span style="--i: 16">e</span>
      <span style="--i: 17">n</span>
      <span style="--i: 18"> </span>
      <span style="--i: 19">B</span>
      <span style="--i: 20">l</span>
      <span style="--i: 21">e</span>
      <span style="--i: 22">u</span>
      <span style="--i: 23">-</span>
    </div>
  </section>
</template>

<style scoped>
section {
  display: flex;
  justify-content: center;
  align-items: center;
  transform-style: preserve-3d;
}

section .sphere {
  position: absolute;
  top: 25vh;
  left: calc(50vw - 7.5rem);
  width: 15rem;
  height: 15rem;
  border-radius: 50%;
  z-index: 10;
  background-color: #d9e0f3;
}

section .sphere::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  z-index: 11;
  border-radius: 50%;
  box-shadow: inset 0 100px 100px rgba(255, 255, 255, 0.5);
  box-shadow: inset 0 -100px 100px rgba(0, 0, 0, 1);
  box-shadow: inset 0 0 100px rgba(0, 0, 0, 1);
}

section .sphere::after {
  content: '';
  position: absolute;
  bottom: -3.7rem;
  left: -3rem;
  width: 25rem;
  height: 5rem;
  border-radius: 50%;
  background: radial-gradient(#000, transparent, transparent);
  z-index: -1;
}

section .sphere img {
  position: absolute;
  height: 80%;
  top: 10%;
  left: 10%;
  border-radius: 50%;
  object-fit: cover;
  filter: blur(0);
}

.circle {
  transform-style: preserve-3d;
  animation: animateText 10s linear infinite;
}

.circle span {
  position: absolute;
  width: 1.5rem;
  min-height: 2rem;
  max-height: 2rem;
  top: 45vh;
  left: -1rem;
  color: #d9e0f3;
  background: #060668;
  font-family: 'Playfair Display', serif;
  font-weight: bold;
  font-size: 2rem;
  transform-origin: center;
  transform-style: preserve-3d;
  padding: 0.5rem;
  transform: rotateY(calc(var(--i) * calc(360deg / 23))) translateZ(9rem);
}

@keyframes animateText {
  0% {
    transform: perspective(50rem) rotateY(360deg) rotateX(0deg);
  }
  100% {
    transform: perspective(50rem) rotateY(0deg) rotateX(0deg);
  }
}

.circle span::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: #060668;
  transform: translateZ(-5px);
}

@media screen and (min-width: 1024px) {
  section .sphere {
    left: calc(50% - 10rem);
    width: 20rem;
    height: 20rem;
  }

  .circle span {
    width: 2.5rem;
    min-height: 3rem;
    max-height: 3rem;
    top: 40vh;
    font-size: 3rem;
    transform: rotateY(calc(var(--i) * calc(360deg / 23))) translateZ(12rem);
  }

  @keyframes animateText {
    0% {
      transform: perspective(50rem) rotateY(360deg) rotateX(0deg);
    }
    100% {
      transform: perspective(50rem) rotateY(0deg) rotateX(0deg);
    }
  }

  .circle span::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: #060668;
    transform: translateZ(-5px);
  }

  section .sphere::after {
    top: 17rem;
    width: 35rem;
    height: 10rem;
  }
}
</style>
