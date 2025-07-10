<template>
    <div class="wrapper">
        <div class="content">
            <div class="text-wrapper">
                <div class="text-header">
                    Static website generator, create websites easily.
                </div>
                <div class="text-info">
                    Generate beautiful, animated, static websites with your creative direction in a matter of minutes. Yes, minutes.
                </div>
                <base-button width="131px" marginRight="10px">Open the App</base-button>
                <base-button backgroundColor="#30B467">Pricing</base-button>
            </div>
            <img class="round" src="../assets/orange_round.svg" alt="round">
            <div class="graphics">
                <img src="../assets/screen.svg" alt="screen">
            </div>
            <img class="rectangle" src="../assets/rectangle.svg" alt="rectangle">
        </div>
        <div class="icons-wrapper"> 
                <img class="icon" src="../assets/1.svg" alt="Logo_Nike">
                <img class="icon" src="../assets/2.svg" alt="Logo_">
                <img class="icon" src="../assets/3.svg" alt="Logo_Microsoft">
                <img class="icon" src="../assets/4.svg" alt="Logo_Ikea">
                <img class="icon" src="../assets/5.svg" alt="Logo_">
                <img class="icon" src="../assets/6.svg" alt="Logo_GoDaddy">
                <img class="icon" src="../assets/7.svg" alt="Logo_Disney">
                <img class="icon" src="../assets/8.svg" alt="Logo_Y">
                <img class="icon" src="../assets/9.svg" alt="Logo_Google">
                <img class="icon" src="../assets/10.svg" alt="Logo_Nasa">
        </div>
    </div>
</template>

<script setup lang="ts">
import BaseButton from './BaseButton.vue';
</script>

<style scoped>
.wrapper {
    width: 100%;
    height: 930px;
    padding-top: 216.88px;
    box-sizing: border-box;
    /* background-color: bisque; */
    
}

.content {
    position: relative;
    /* background-color: aliceblue; */
    box-sizing: border-box;
    width: calc(100% - 260px); /*83%*/ 
    height: 365.875px;
    margin-bottom: 200px;
    margin-left: 120.19px;
    margin-right: 33px;
    padding-left: 9.81px;
    padding-right: 9.81px;
    display: flex; 
    align-items: center; 
    justify-content: space-between;
}

.text-wrapper {
    /* background-color: greenyellow; */
    width: 42%;
    height: 343px;
    padding-left: 9.81px;
    z-index: 2; /* выше круга */
}

.text-header {
    /* background-color: goldenrod; */
    width: 61.16%;
    height: 169px;
    overflow: hidden;

    font-family: Roboto;
    font-weight: 400;
    font-style: Regular;
    font-size: 45px;
    line-height: 56.25px;
    letter-spacing: 0.99px;
    margin-bottom: 20px;
    
    
}

.text-info {
    /* background-color: bisque; */
    width: 72.75%;
    height: 95px;
    overflow: hidden;

    font-family: Roboto;
    font-weight: 400;
    font-style: Regular;
    font-size: 21px;
    line-height: 31.5px;
    letter-spacing: 0.23px;

}

.round {
    position: absolute;
    width: 200px; 
    height: 200px;
    /* left: 61.88%; 
    transform: translateX(-50%); */
    left: 60%; /* двигает влево */
    top: 50%;
    transform: translate(-50%, -50%);

}

.graphics {
    /* background-color: blueviolet; */
    width: 580PX;
    height: 366PX;

    z-index: 2; 
}

.rectangle {
    position: absolute;
    top: 79.5%;
    right: -30px; 
    transform: translateY(-50%);
    z-index: 3; 
}

.icons-wrapper {
    width: calc(100% - 260px);
    overflow: hidden;
    margin: 0 130.19px;
    height: 68px;
    top: 851.88px;
    left: 130.19px;
    /* background-color: blue; */
    display: flex; 
    align-items: center; 
    justify-content: space-between;
}
/* .icon {
    background-color: rgb(163, 105, 29); 
} */

</style>