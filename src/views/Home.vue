<template>
    <section>
      <h1>Welcome to Your Vue TypeScript Website</h1>
      <p>This is the main section of your website.</p>
    </section>
  </template>
  
  <script lang="ts">
  import { Component, Vue } from 'vue';
  
  @Component
  export default class Home extends Vue {}
  </script>