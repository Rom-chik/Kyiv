<script setup lang="ts">
import Navigation from './components/Navigation.vue'
import SideScrollCards from './components/SideScrollCards.vue'
import Timestamps from './components/Timestamps.vue'
</script>

<template>
  <!-- Header -->
  <div class="flex justify-center items-center w-full h-[40vh] text-9xl">
      K y i v
  </div>

  <!-- Navigations Menu -->
  <div class="flex w-full justify-center items-center h-[70vh]">
      <Navigation/>
  </div>
  <!-- Timestamps -->
  <div class="flex w-full gap-5 justify-center items-center h-[50vh]">
      <Timestamps/>
  </div>

  <!-- Side scroll cards -->
  <div class="w-full h-[100vh] bg-[#F0F0F0]">
      <div class="side-scroll flex h-full justify-between gap-10 items-center">
          <SideScrollCards/>
      </div>
  </div>

  <!-- Bottom -->
  <div class="flex w-full h-[70vh]">

  </div>
</template>

<style scoped>
    .side-scroll{
        display: flex;
        flex-wrap: nowrap;
        overflow: auto;
      padding: 0; /* Reset padding if any */
      margin: 0;
    }
</style>
