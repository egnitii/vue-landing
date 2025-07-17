<template>
  <div class="wrapper">
    <HeaderMain></HeaderMain>
    <main>
      <FirstPart></FirstPart>
    </main>
    <!-- <footer></footer> -->
  </div>
</template>

<script setup lang="ts">
import HeaderMain from "./components/HeaderMain.vue"
import FirstPart from "./components/FirstPart.vue"
</script>

<style>
.wrapper {
  margin-top: 10px;
}
</style>