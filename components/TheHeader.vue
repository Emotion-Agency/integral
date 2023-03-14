<script setup lang="ts">
const isOpened = ref(false)

const onClick = () => {
  isOpened.value = !isOpened.value
}
</script>

<template>
  <header class="header">
    <div class="container header__wrapper">
      <NuxtLink to="/" class="header__logo">Integral</NuxtLink>
      <button class="header__btn" @click="onClick">
        {{ !isOpened ? 'Menu' : 'Close' }}
      </button>
    </div>
  </header>
  <PopupMenu :open="isOpened" />
</template>
