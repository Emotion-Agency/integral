<script setup lang="ts"></script>

<template>
  <footer class="footer">
    <div class="container footer__wrapper">
      <div class="footer__email">
        <h3 class="footer__title">
          Let’s talk
          <span class="footer__arrow">
            <IconsAngleArrow />
          </span>
        </h3>
        <TheButton class="footer__btn">info@integral.im</TheButton>
      </div>
      <div class="grid footer__content">
        <p class="footer__about">Integral © 2018 ⸺ 2023</p>
        <ul class="footer__nav-menu">
          <li class="footer__nav">
            <NuxtLink to="/">About</NuxtLink>
          </li>
          <li class="footer__nav">
            <NuxtLink to="/">Studio</NuxtLink>
          </li>
          <li class="footer__nav">
            <NuxtLink to="/">Services</NuxtLink>
          </li>
          <li class="footer__nav">
            <NuxtLink to="/">Approach</NuxtLink>
          </li>
          <li class="footer__nav">
            <NuxtLink to="/">Contact</NuxtLink>
          </li>
        </ul>
        <ul class="footer__socials-menu">
          <li class="footer__social">
            <a
              href="/"
              class="footer__link"
              rel="noopener noreferrer"
              target="_blank"
            >
              Instagram
            </a>
          </li>
          <li class="footer__social">
            <a
              href="/"
              class="footer__link"
              rel="noopener noreferrer"
              target="_blank"
            >
              LinkedIn
            </a>
          </li>
          <li class="footer__social">
            <a
              href="/"
              class="footer__link"
              rel="noopener noreferrer"
              target="_blank"
            >
              Twitter
            </a>
          </li>
        </ul>
        <p class="footer__text-info">Beauty lies in the details</p>
      </div>
    </div>
  </footer>
</template>
