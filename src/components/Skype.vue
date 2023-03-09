<script setup>
import SideBar from './Sidebar/SideBar.vue';
import ChatSection from './ChatSection.vue'
</script>
<template>
  <div class="container">
    <SideBar />
    <ChatSection />
  </div>
</template>

<style>
.container {
  width: 96rem;
  height: 54rem;
  border: .1rem solid var(--border-color);
  background: rgba(255, 255, 255, .08);
  box-shadow: 0px .2rem 12.5rem rgba(255, 255, 255, .1);
  backdrop-filter: blur(40px);
  border-radius: 1rem;
  display: grid;
  grid-template-columns: 17.5rem 78.5rem;
}

/* .container::after{
  content: '';
  position: absolute;
  inset: 0;
  background-color: rgba(255,255,255,.08);
  backdrop-filter: blur(5px);
  box-shadow: inset 0 0 0 150rem rgba(255, 255, 255, .08);
} */
</style>