<template>
    <button 
        class="base-button"
        :style="{ 
            backgroundColor ,
            width,
            marginRight
            }"
    > 
        <slot> </slot> 
    </button>
</template>

<script setup lang="ts">
import { defineProps } from 'vue'

const props = defineProps({
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

    font-family: 'Roboto', sans-serif;
    font-weight: 400;
    font-style: regular;
    font-size: 15px;
    line-height: 22.5px;
}
</style>