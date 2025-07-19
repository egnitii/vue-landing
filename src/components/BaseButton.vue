<template>
    <button 
        class="base-button text"
        :style="{ 
            backgroundColor ,
            width,
            marginRight
            }"
    > 
    <slot></slot>
      <!-- <slot></slot> можно делать одиночным, мб конфигурации обновить -->
    </button>
</template> 

<script setup lang="ts">
defineProps({
  backgroundColor: {
    type: String,
    default: '#2164E1',
  },
  width: {
    type: String,
    default: '74px',
  },
  marginRight: {
    type: String,
    default: '0px',
  },
})
</script>

<style>
.base-button {
    height: 42px;
    top: 4%;
    border-radius: 6px;
    color: white;
    border: none;
    cursor: pointer;
    margin-top: 15px;
}
</style>