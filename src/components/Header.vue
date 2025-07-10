<template>
  <div class="header">
    <div class="header-inside">
      <div class="logo">
        <Logo></Logo>
      </div>
      <div class="menu">
        <div class="items">
          <div class="item my-text"> Pricing </div>
          <div class="item my-text"> Help </div>
          <div class="item my-text"> Login </div>
        <BaseButton> Demo </BaseButton>
        </div>
      </div>
      
    </div>
  </div>
</template>

<script setup>
import Logo from "./Logo.vue"
import BaseButton from "./BaseButton.vue";
</script>

<style scoped>
.header {
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
  }
}



.logo {
  position: relative;
  top: 5px;
  width: 101px;
  height: 35px;

  display: flex;
}
.menu {
  position: relative;
  right: 0px;
  width: 590px;
  height: 50px;

  display: flex;
  align-items: center;
  gap: 20px;
}

/* .button-demo {
  width: 74px;
  height: 42px;
  top: 4%;
  border-radius: 6px;
  color: white;
  border: none;
  background-color: #2164E1;
  cursor: pointer;
} */

.items {
  position: absolute;
  width: 248px;
  height: 20px;
  top: 13.36px;
  left: 263px;

  display: flex;
  gap: 20px;
  align-items: center;
}

.my-text {
  font-family: 'Roboto', sans-serif;
  font-weight: 400;
  font-style: normal;
  font-size: 16px;
  line-height: 24px;
  letter-spacing: 0;

}

/* .text-button {
  font-style: regular;
  font-size: 15px;
  line-height: 22.5px;
} */

.item {
  height: 20px;
}
</style>