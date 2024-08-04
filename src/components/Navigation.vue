<script setup lang="ts">

</script>

<template>
  <div class="flex justify-evenly flex-wrap gap-[10vw]">
    <div class="dropdown">
      <button class="menu--button text-4xl peer">Options</button>
      <div class="content text-2xl peer-focus:block">
        <a href="#">option 1</a>
        <a href="#">option 2</a>
        <a href="#">option 3</a>
      </div>
    </div>
    <div class="dropdown">
      <button class="menu--button text-4xl peer">Menu</button>
      <div class="content text-2xl peer-focus:block">
        <a href="#">option 1</a>
        <a href="#">option 2</a>
        <a href="#">option 3</a>
      </div>
    </div>
    <div class="dropdown">
      <button class="menu--button text-4xl peer">More</button>
      <div class="content text-2xl peer-focus:block">
        <a href="#">option 1</a>
        <a href="#">option 2</a>
        <a href="#">option 3</a>
      </div>
    </div>
  </div>
</template>

<style scoped>
.dropdown a{
  display: block;
  padding: 10px 10px 10px 25px;
  width: 100%;
}
.dropdown a:hover{
  background: RGBA(255, 255, 255, 0.7);
  border-radius: 10px;
}
.content{
  display: none;
  position: absolute;
  background: RGBA(220, 220, 220, 0.5);
  border-radius: 10px;
  min-width: 140px;
  padding: 5px;
  margin-top: 10px;
}

.menu--button{
  padding: 10px;
}
.menu--button:hover{
  padding: 10px;
  cursor: pointer;
  border-radius: 10%;
}
</style>