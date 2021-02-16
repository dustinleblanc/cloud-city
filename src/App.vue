<template>
  <div class="h-screen w-screen flex flex-col pt-12">
    <TopBar />
    <!-- [ HERE COMES YOUR CONTENT ] -->
    <transition name="fade" appear>
      <div class="flex flex-col items-center justify-center h-full pb-0">
        <img class="h-48 ml-5" src="/logo.png" draggable="false" />
      </div>
    </transition>
    <app-waves></app-waves>
  </div>
</template>

<script>
import TopBar from '/~/components/layout/TopBar.vue'
import AppWaves from '/~/components/effects/AppClouds.vue'

export default {
  name: 'App',
  components: {
    AppWaves,
    TopBar,
  },
}
</script>
