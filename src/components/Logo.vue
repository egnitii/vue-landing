<template>
    <div>
        <img class="pic-logo" src="../assets/logo.svg" alt="logo">
        <img class="pic-round" src="../assets/round.svg" alt="round">
        <img class="pic-five" src="../assets/5l.svg" alt="five">
    </div>
</template>

<script>
    export default {
        name: "Logo"
    }

</script>

<style  scoped>


.pic-logo {
  position: absolute;
  top: 11px;
  width: 83.2px;
  height: 24px;
}

.pic-round {
  position: absolute;
  width: 18px;
  height: 18px;
  left: 83px;
  opacity: 90%;
}

.pic-five {
  position: absolute;
  width: 5.13px;
  height: 8.11px;
  left: 89.5px;
  top: 5px;
}
</style>