<template>
  <header class="frame">
    <div class="rectangle"></div>
    <div class="inner-frame">
    <h1>привет медвед</h1>   </div>

  </header>
</template>

<style scoped>
.frame {
  position: relative;
  height: 70px;
  width: 100%;
}

.rectangle {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;

  height: 70px;
  background: rgba(255, 255, 255, 0.976);
  box-shadow: 0px 1px 1px rgba(0, 0, 0, 0.07);
  border-radius: 0;

  z-index: 0;
}

.inner-frame {
  margin: 10px 9.03% 0 9.03%; 
  height: 50px;
}


</style>
