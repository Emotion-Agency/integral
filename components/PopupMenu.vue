<script setup lang="ts">
interface iProps {
  open: boolean
}
defineProps<iProps>()
</script>

<template>
  <div class="popup" :class="open && 'popup--opened'">
    <div class="popup-backdrop"></div>
    <div class="popup__wrapper">
      <ul class="popup__nav-menu">
        <li class="popup__nav">
          <NuxtLink to="/">About</NuxtLink>
        </li>
        <li class="popup__nav">
          <NuxtLink to="/">Studio</NuxtLink>
        </li>
        <li class="popup__nav">
          <NuxtLink to="/">Services</NuxtLink>
        </li>
        <li class="popup__nav">
          <NuxtLink to="/">Approach</NuxtLink>
        </li>
        <li class="popup__nav">
          <NuxtLink to="/">Contact</NuxtLink>
        </li>
      </ul>
      <ul class="popup__socials-menu">
        <li class="popup__social">
          <a
            href="/"
            class="popup__link"
            rel="noopener noreferrer"
            target="_blank"
          >
            Instagram
          </a>
        </li>
        <li class="popup__social">
          <a
            href="/"
            class="popup__link"
            rel="noopener noreferrer"
            target="_blank"
          >
            LinkedIn
          </a>
        </li>
        <li class="popup__social">
          <a
            href="/"
            class="popup__link"
            rel="noopener noreferrer"
            target="_blank"
          >
            Twitter
          </a>
        </li>
      </ul>
    </div>
  </div>
</template>
