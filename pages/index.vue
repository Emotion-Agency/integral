<script setup lang="ts">
import { pageTransition } from '~~/assets/scripts/transition'

definePageMeta({
  pageTransition,
})
</script>

<template>
  <section class="section section--nm home-1">
    <img class="home-1__bg" src="/images/main.jpg" alt="Background" />
    <div class="container home-1__wrapper">
      <h1 class="home-1__title">
        A multidisciplinary creative consultancy shaping
        <span class="home-1__underline-text"> digital culture </span>
      </h1>
    </div>
  </section>
  <section class="section section--nm home-2">
    <div class="container home-2__wrapper">
      <p class="home-2__about-text">
        Empowering brands at the forefront of digital
        <span class="home-2__arrow">
          <IconsAngleArrow />
        </span>
      </p>
      <p class="home-2__text">
        Integral is a multi-disciplinary design studio, catalysing insights with
        technology to build thoughtful
        <span class="home-2__underline-text">design-led solutions</span> for
        dynamic global clients. <br /><br />
        From strategy, to creative direction and production, we deliver
        innovative and engaging experiences that
        <span class="home-2__underline-text"
          >connect brands with their audiences.</span
        >
      </p>
    </div>
  </section>
  <section class="section section--nm home-3">
    <HomeVideo class="home-3__bg" />
  </section>
  <section class="section section--nm home-4">
    <div class="container home-4__wrapper">
      <p class="home-4__about-text">
        About
        <span class="home-4__arrow">
          <IconsAngleArrow />
        </span>
      </p>
      <div class="grid home-4__content">
        <div class="home-4__left-block">
          <h2 class="home-4__title">
            Redefining brand dimensionalities
            <span class="home-4__title-arrow">
              <IconsAngleArrow />
            </span>
          </h2>
          <div class="home-4__text-wrapper">
            <p class="home-4__med-desc">
              Operating at the intersection of physical & digital, specialising
              in; <span class="home-4__underline-text">brand</span>,
              <span class="home-4__underline-text">fashion</span>,
              <span class="home-4__underline-text">product</span> &
              <span class="home-4__underline-text">web3</span>.
            </p>
            <p class="home-4__small-desc">
              With deep knowledge broadly spanning design, fashion & web3, we
              help our partners grow through our innate understanding of the
              drivers behind tomorrow’s trends and opportunities.
            </p>
          </div>
          <div class="home-4__btn-wrapper">
            <TheButton> Studio </TheButton>
          </div>
        </div>
        <div class="home-4__right-block">
          <img class="home-4__img" src="/images/1.jpg" alt="Image" />
        </div>
      </div>
    </div>
  </section>
  <section class="section section--nm home-5">
    <div class="container home-5__wrapper"></div>
  </section>
</template>
