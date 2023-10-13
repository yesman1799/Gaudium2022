<template>
    <section>
      <h2>Contact Us</h2>
      
      <form @submit.prevent="submitForm">
        <label for="name">Name:</label>
        <input type="text" id="name" v-model="name" required>
        
        <label for="email">Email:</label>
        <input type="email" id="email" v-model="email" required>
        
        <label for="message">Message:</label>
        <textarea id="message" v-model="message" rows="4" required></textarea>
        
        <button type="submit">Submit</button>
      </form>
    </section>
  </template>
  
  <script lang="ts">
  import { Component, Vue } from 'vue';
  
  @Component
  export default class Contact extends Vue {
    name: string = '';
    email: string = '';
    message: string = '';
  
    submitForm(): void {
      // You can add form submission logic here
      console.log('Form submitted:', this.name, this.email, this.message);
    }
  }
  </script>
  
  <style scoped>
    section {
      padding: 50px;
      text-align: center;
    }
  
    form {
      max-width: 600px;
      margin: 0 auto;
    }
  
    label {
      display: block;
      margin-bottom: 8px;
    }
  
    input, textarea {
      width: 100%;
      padding: 10px;
      margin-bottom: 20px;
      box-sizing: border-box;
    }
  
    button {
      background-color: #3498db;
      color: white;
      padding: 10px 20px;
      border: none;
      cursor: pointer;
    }
  </style>
  