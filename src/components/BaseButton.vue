<template>
    <button class="base-button"> 
        <slot> </slot> 
    </button>
</template>

<script setup>
    
</script>

<style scoped>
.base-button {
    width: 74px;
    height: 42px;
    top: 4%;
    border-radius: 6px;
    color: white;
    border: none;
    background-color: #2164E1;
    cursor: pointer;

    font-family: 'Roboto', sans-serif;
    font-weight: 400;
    font-style: regular;
    font-size: 15px;
    line-height: 22.5px;
}
</style>