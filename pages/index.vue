<template>
  <div class="my-element">
    Welcome
  </div>
</template>

<script setup>
import { onMounted } from 'vue'
import { useNuxtApp } from '#app'

onMounted(() => {
  const { $gsap } = useNuxtApp()
  
  $gsap.to('.my-element', {
    rotation: 360,
    duration: 2,
    ease: 'bounce.out'
  })
})
</script>