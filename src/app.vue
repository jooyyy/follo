<template>
  <div class="container">
    <UINav />
    <UICalender />
  </div>
</template>
<script setup lang="ts">
</script>
<style>
body{
  margin: 0;
}
.container {
  display: flex;
  height: 100vh;
  width: 100%;
  background-color: #f8f9fa;
  transition: width var(--transition-duration) var(--transition-timing-function);
  --transition-duration: 300ms;
  --delayed-transition-duration: 400ms;
  --transition-timing-function: cubic-bezier(0, 0, 0, 1);
}
</style>
