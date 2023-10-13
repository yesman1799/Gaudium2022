<template>
  <div id="app">
    <nav>
      <ul>
        <li><router-link to="/">Home</router-link></li>
        <li><router-link to="/contact">Contact</router-link></li>
      </ul>
    </nav>
    
    <router-view/>

    <footer>
      <p>&copy; 2023 Your Website</p>
    </footer>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue';

@Component
export default class App extends Vue {}
</script>

<style>
#app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    text-align: center;
    color: #2c3e50;
  }

  nav {
    background-color: #3498db;
    padding: 15px;
    color: white;
  }

  ul {
    list-style-type: none;
    padding: 0;
  }

  li {
    display: inline;
    margin-right: 20px;
  }

  a {
    text-decoration: none;
    color: white;
    font-weight: bold;
  }

  footer {
    margin-top: 50px;
    padding: 10px;
    background-color: #ecf0f1;
  }
</style>
