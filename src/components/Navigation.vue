<script setup lang="ts">

</script>

<template>
  <div class="w-[70vw] h-[70vh] grid grid-rows-12 grid-cols-3 gap-5">
      <div class="row-start-2 row-end-12 nav-button">
          <div class="text-5xl">Options</div>
          <div class="dropup">
              <a href="#">Light/dark theme</a>
              <a href="#">Mobile/PC</a>
              <a href="#">Language</a>
          </div>
      </div>
      <div class="row-start-1 row-end-10 nav-button">
          <div class="dropdown">
              <a href="#">Clock</a>
              <a href="#">Photo set</a>
              <a href="#">Work in process</a>
          </div>
          <div class="text-5xl">Menu</div>
      </div>
      <div class="row-start-4 row-end-13 nav-button">
          <div class="text-5xl">More</div>
          <div class="dropup">
            <a href="#">GitHub</a>
            <a href="#">Instagram</a>
            <a href="#">@Email</a>
          </div>
      </div>
  </div>
</template>

<style scoped>
    .nav-button {
      border-width: 4px;
      border-color: black;
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
    .nav-button:has(.dropdown):hover {
      background-color: black;
      color: white;
      padding-top: 40px;
    }
    .nav-button:has(.dropup):hover {
      background-color: black;
      color: white;
      padding-bottom: 40px;
    }
    .dropdown {
      display: none;
      flex-direction: column;
      align-items: center;
      margin-top: 50px;
      margin-bottom: 50px;
      transition: opacity 1s;
    }
    .dropup {
      display: none;
      flex-direction: column;
      align-items: center;
      margin-top: 50px;
      margin-bottom: 50px;
      transition: opacity 1s;
    }
    .nav-button:hover .dropdown {
      display: flex;
      opacity: 1;
    }
    .nav-button:hover .dropup {
      display: flex;
      opacity: 1;
    }
    a {
      margin: 5px 0;
      color: black;
      transition: color 0.7s;
      border: 2px solid transparent;
      width: 150px;
      padding: 5px 5px 5px 20px;
    }
    .nav-button:hover a {
      color: white;
    }
    .nav-button:hover a:hover {
      box-sizing: border-box;
      border: 2px solid #717171;
      border-radius: 10px;
    }
    a:active {
      box-sizing: border-box;
      border: 2px solid #717171;
      background: #717171;
      border-radius: 10px;
    }
</style>