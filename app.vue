<template>
  <div class="app">
    <div class="app_box">
      <NuxtLayout>
        <NuxtPage/>
      </NuxtLayout>
    </div>
  </div>
</template>

<script setup>
definePageMeta({
  layout: 'default'
})
</script>

<style lang="less">
body {
  margin: 0;
  background-color: #0C0E14;
  color: white;
}

.app {
  padding: 50px;
  display: flex;
  justify-content: center;

  .app_box {
    width: 1200px;
    position: relative;
  }
}
</style>