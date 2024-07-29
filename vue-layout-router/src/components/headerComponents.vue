<template>
    <header>
      <h1>{{ title }}</h1>
      <img src="./assets/logo.png" alt="Logo">
    </header>
  </template>
  
  <script>
  export default {
    name: 'HeaderComponent',
    data() {
      return {
        title: 'Meu Site Incrível'  
      };
    }
  };
  </script>
  
  <style scoped>

  header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1rem;
    background-color: #333;
    color: white;
  }
  h1 {
    margin: 0;
  }
  img {
    height: 50px; 
  }
  </style>