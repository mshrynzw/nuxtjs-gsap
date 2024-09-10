<template>
  <div class="box">
    <div class="p-8 text-white bg-blue-500">
      Welcome
    </div>
  </div>
</template>

<script setup>
import {onMounted} from 'vue'
import {useNuxtApp} from '#app'

onMounted(() => {
  const {$gsap} = useNuxtApp()

  $gsap.to(".box", {x: 200})
})
</script>