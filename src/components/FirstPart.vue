<template>
    <div class="wrapper-content">
        <section class="content">
            <div class="text-wrapper text">
                <h1 class="text-header">Static website generator, create websites easily.</h1>
                <p class="text-info"> Generate beautiful, animated, static websites with your creative direction in a matter of minutes. Yes, minutes. </p>
                <base-button width="131px" marginRight="10px">Open the App</base-button>
                <base-button backgroundColor="#30B467">Pricing</base-button>
            </div>
            <div class="screen-wrapper">
                <img class="screen" src="../assets/icons/screen.svg" alt="screen">
            </div>
        </section>
        <section class="icons-wrapper"> 
            <img 
                v-for="icon in icons"
                :key="icon.name"
                :src="icon.component" 
                :alt="icon.name"
                class="icon"
            />
        </section>
        <registration-form></registration-form>
    </div>
</template>

<script setup lang="ts">
import RegistrationForm from './RegistrationForm.vue';
import BaseButton from './BaseButton.vue';
import Logo_Nike from "../assets/icons/1.svg";
import Logo_A from "../assets/icons/2.svg";
import Logo_Microsoft from "../assets/icons/3.svg";
import Logo_Ikea from "../assets/icons/4.svg";
import Logo_T from "../assets/icons/5.svg";
import Logo_GoDaddy from "../assets/icons/6.svg";
import Logo_Disney from "../assets/icons/7.svg";
import Logo_Y from "../assets/icons/8.svg";
import Logo_Google from "../assets/icons/9.svg";
import Logo_Nasa from "../assets/icons/10.svg";

const icons = [
    { name: "Logo_Nike", component: Logo_Nike},
    { name: "Logo_A", component: Logo_A},
    { name: "Logo_Microsoft", component: Logo_Microsoft},
    { name: "Logo_Ikea", component: Logo_Ikea},
    { name: "Logo_T", component: Logo_T},
    { name: "Logo_GoDaddy", component: Logo_GoDaddy},
    { name: "Logo_Disney", component: Logo_Disney},
    { name: "Logo_Y", component: Logo_Y},
    { name: "Logo_Google", component: Logo_Google},
    { name: "Logo_Nasa", component: Logo_Nasa},
]
</script>

<style>
.wrapper-content {
    width: 100%;
    height: 930px;
    padding-top: 216.88px;
    box-sizing: border-box;
    /* background-color: bisque; */

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

        .text-wrapper {
            /* background-color: greenyellow; */
            width: 42%;
            height: 343px;
            padding-left: 9.81px;
           
            z-index: 2; /* выше круга */

            .text-header {
                /* background-color: goldenrod; */
                width: 61.16%;
                height: 169px;
                overflow: hidden;

                font-size: 45px;
                line-height: 56.25px;
                letter-spacing: 0.99px;
                margin-bottom: 22px;
                
                
            }

            .text-info {
                /* background-color: bisque; */
                width: 72.75%;
                height: 95px;
                overflow: hidden;

                font-size: 21px;
                line-height: 31.5px;
                letter-spacing: 0.23px;
            }
        }

        .screen-wrapper {
            /* background-color: blueviolet; */
            width: 580PX;
            height: 366PX;
            
        }

        .screen-wrapper::before {
            content: '';
            position: absolute;
            width: 200px;
            height: 200px;
            top: 95px;
            left: -76.98px;
            opacity: 1;
            border-radius: 999px;
            background: rgba(242, 80, 34, 1);
            box-shadow: 0px 8px 13px 0px rgba(242, 80, 34, 0.2);           
            top: 50%;
            left: 60%;
            transform: translate(-50%, -50%);
            z-index: 1; 
            

        }
        .screen {
            position: relative;
            z-index: 2; 
        }
        
        .screen-wrapper::after {
            content: '';
            position: absolute;
            width: 65px;
            height: 47px;
            top: 87%;                
            left: 93.5%;              /* ставим сразу за изображением */
            margin-left: 20px;   
            opacity: 1;
            border-radius: 10px;
            background: rgba(33, 100, 225, 1);
            box-shadow: 0px 8px 13px 0px rgba(33, 100, 225, 0.2);
            transform: translateY(-50%);
            z-index: 3;
        }
    }

    .icons-wrapper {
        width: calc(100% - 260px);
        overflow: hidden;
        margin: 0 130.19px;
        height: 68px;
        top: 851.88px;
        left: 130.19px;
        display: flex; 
        align-items: center; 
        justify-content: space-between;
        /* background-color: blue; */
        /* .icon {
            background-color: rgb(163, 105, 29); 
        } */
    }   
}


</style>