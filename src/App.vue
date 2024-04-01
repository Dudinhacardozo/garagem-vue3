<script setup>
import router from './router';
</script>
<template>
  <header>
    <router-link :to="{ name: 'home' }">Home</router-link> |
    <router-link to="/acessorios">Acessórios</router-link> |
    <router-link to="/categorias">Categorias</router-link> |
    <router-link to="/cores">Cores</router-link> |
    <router-link to="/marcas">Marcas</router-link> 
  </header>
  <main>
    <router-view />
  </main>
</template>


<style>
  body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
  }

  header {
    background-color: #333;
    color: #fff;
    padding: 10px;
    text-align: center;
  }

  header a {
    color: #fff;
    text-decoration: none;
    margin: 0 10px;
    transition: all 0.3s ease;
  }

  header a:hover {
    text-decoration: underline;
  }

  main {
    padding: 20px;
  }

  main a {
    display: block;
    color: #007bff;
    text-decoration: none;
    padding: 10px;
    margin-bottom: 10px;
    background-color: #f4f4f4;
    border-radius: 5px;
    transition: all 0.3s ease;
  }

  main a:hover {
    background-color: #ddd;
  }

  .RouterView-enter-active, .RouterView-leave-active {
    transition: opacity 0.5s;
  }

  .RouterView-enter, .RouterView-leave-to {
    opacity: 0;
  }
</style>