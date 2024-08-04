<script setup lang="ts">
import Navigation from './components/Navigation.vue'
import SideScrollCards from './components/SideScrollCards.vue'
</script>

<template>
  <!-- Header -->
  <div class="flex justify-center items-center w-full h-[40vh] text-9xl">
      K y i v
  </div>

  <!-- Navigations Menu -->
  <div class="flex w-full justify-center items-baseline h-[90vh]">
      <Navigation/>
  </div>
  <!-- Timestamps -->
  <div class="flex w-full h-[50vh]">

  </div>

  <!-- Side scroll cards -->
  <div class="w-full h-[100vh] bg-[#F0F0F0]">
      <div class="side-scroll flex h-full justify-around gap-10 items-center">
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
