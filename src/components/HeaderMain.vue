<template>
  <header>
    <div class="header-inside"> 
      <div class="logo">
        <Logo></Logo>
      </div>
      <nav>
        <div class="items">
          <button class="item text">Pricing</button>
          <button class="item text">Help</button>
          <button class="item text">Login</button>
        <BaseButton> Demo </BaseButton>
        </div>
      </nav>
    </div>
  </header>
</template>

<script setup lang="ts">
import Logo from "./Logo.vue"
import BaseButton from "./BaseButton.vue";
</script>

<style>
header {
  position: relative;
  width: 100%;
  height: 70px;
  
  .header-inside {
    position: absolute;
    top: 10px;
    left: 130px;
    right: 130px;
    height: 50px;
    
    display: flex;
    justify-content: space-between;
    align-items: center;
    
    .logo {
      position: relative;
      top: 5px;
      width: 101px;
      height: 35px;

      display: flex;
    }

    nav {
      position: relative;
      right: 0px;
      width: 590px;
      height: 50px;

      display: flex;
      align-items: center;
      gap: 20px;

      .items {
        position: absolute;
        width: 248px;
        height: 20px;
        top: 13.36px;
        left: 263px;

        display: flex;
        gap: 20px;
        align-items: center;
        
        .text {
          font-style: normal;
          font-size: 16px;
          line-height: 24px;
          letter-spacing: 0;
        }
        
        .item {
          height: 20px;
          cursor: pointer;
        }
      }
    }
  }
}
</style>