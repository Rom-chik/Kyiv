<script setup lang="ts">
    import { useCurrentTime } from '../composables/useCurrentTime';

    const { currentTime } = useCurrentTime();
    console.log(currentTime.value);

    const options = {
      weekday: 'long',
      year: 'numeric',
      month: 'long',
      day: 'numeric',
    };
</script>

<template>
    <div class="w-full flex flex-col gap-20">
        <div class="w-full h-[10px] bg-black"></div>
        <div class="w-full h-[10px] bg-black"></div>
    </div>
    <div class="flex justify-around items-center">
          <div class="w-1/6">
              <div class="text-2xl">{{ currentTime.toLocaleDateString(undefined, options) }}</div>
          </div>
          <div class="justify-center w-4/6">
              <div class="text-8xl">{{ currentTime.toLocaleTimeString() }}</div>
          </div>
          <div class="w-1/6">
              <div class="text-2xl">Geo + Weather</div>
          </div>
    </div>
    <div class="w-full flex flex-col gap-20">
        <div class="w-full h-[10px] bg-black"></div>
        <div class="w-full h-[10px] bg-black"></div>
    </div>
</template>

<style scoped>

</style>