<script setup lang="ts">

</script>

<template>
  <div class="w-[70vw] h-[70vh] grid grid-rows-12 grid-cols-3 gap-5">
      <div class="row-start-2 row-end-12 nav-card border-4 border-black dark:border-white">
          <div class="text-5xl pb-5">Options</div>
          <div class="dropup text-white dark:text-black">
              <button @click="$emit('switch-theme')">Light/dark theme</button>
              <button>Mobile/PC</button>
              <button>Language</button>
          </div>
      </div>
      <div class="row-start-1 row-end-10 nav-card border-4 border-black dark:border-white">
          <div class="dropdown text-white dark:text-black">
              <a href="#clock">Clock</a>
              <a href="#photo-set">Photo set</a>
              <a href="#work-in-process">Work in process</a>
          </div>
          <div class="text-5xl pt-4">Menu</div>
      </div>
      <div class="row-start-4 row-end-13 nav-card border-4 border-black dark:border-white">
          <div class="text-5xl pb-5">More</div>
          <div class="dropup text-white dark:text-black">
            <a href="#">GitHub</a>
            <a href="#">Instagram</a>
            <a href="#">@Email</a>
          </div>
      </div>
  </div>
</template>

<style scoped>
    .nav-card {
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      cursor: pointer;
      transition: background-color 0.7s, color 0.7s, height 1s, padding-top 1s, padding-bottom 1s;
      padding-top: 0;
      padding-bottom: 0;
      overflow: hidden;
      position: relative;
    }
    .nav-card:has(.dropdown):hover {
      background-color: black;
      color: white;
      padding-top: 40px;
    }
    .nav-card:has(.dropup):hover {
      background-color: black;
      color: white;
      padding-bottom: 40px;
    }
    .dropdown {
      display: flex;
      flex-direction: column;
      align-items: center;
      margin-top: 10px;
      margin-bottom: 10px;
      transition: opacity 1s;
    }
    .dropup {
      display: flex;
      flex-direction: column;
      align-items: center;
      margin-top: 10px;
      margin-bottom: 10px;
      transition: opacity 1s;
    }
    .nav-card:hover .dropdown {
      display: flex;
      opacity: 1;
    }
    .nav-card:hover .dropup {
      display: flex;
      opacity: 1;
    }
    a, button {
      margin: 5px 0;
      transition: color 0.7s;
      border: 2px solid transparent;
      width: 150px;
      padding: 5px 5px 5px 20px;
    }
    .nav-card:hover a, .nav-card:hover button {
      color: white;
      transition: color 1s;
    }
    .nav-card:hover a:hover, .nav-card:hover button:hover {
      box-sizing: border-box;
      border: 2px solid #3D3D3D;
      border-radius: 10px;
    }
    a:active, button:active{
      box-sizing: border-box;
      border: 2px solid #717171;
      background: #3D3D3D;
      border-radius: 10px;
    }
</style>