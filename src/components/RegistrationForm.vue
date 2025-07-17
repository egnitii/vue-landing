<template>
  <div class="form-wrapper">
    <h2 class=" text side-text"> If you want to work with real professionals – leave a request, and you’ll get all the details.</h2>
    <div class="form">
      <input
        v-model="phone"
        type="tel"
        placeholder="Enter your phone number"
        class="input text"
      />

      <button
        class="submit-btn text"
        @click="handleSubmit"
        :disabled="isSubmitting"
      >
        {{ isSubmitting ? "Loading..." : "Leave a request" }}
      </button>

      <p v-if="message" class="message text">
        {{ message }}
      </p>
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue'

const phone = ref('')
const message = ref('')
const isSubmitting = ref(false)

function handleSubmit() {
  if (!phone.value.trim()) {
    message.value = 'Please, enter your phone number'
    return
  }

  isSubmitting.value = true
  message.value = ''

  setTimeout(() => {
    isSubmitting.value = false
    message.value = 'Application sent successfully!'
    phone.value = ''
  }, 1500)
}
</script>

<style>

.form-wrapper {
    display: flex;
    align-items: flex-start;
    gap: 40px;
    max-width: 800px;
    width: 100%; 
    margin: 0 auto 0;
    padding-top: 100px;
    padding-bottom: 100px;

    .side-text {
        flex: 1;
        font-size: 28px;
        line-height: 28px;
        color: #000000;        
    }

    .form {
        flex: 1;
        display: flex;
        flex-direction: column;
        gap: 12px;
        max-width: 300px;

        .input {
            padding: 10px;
            font-size: 16px;
        }

        .submit-btn {
            padding: 10px;
            background-color: #2164E1;
            color: white;
            border: none;
            border-radius: 6px;
            cursor: pointer;
        }

        .submit-btn:disabled {
            background-color: #94b8f3;
            cursor: not-allowed;
        }

        .message {
            color: green;
            font-size: 14px;
        }
    }
}
</style>
