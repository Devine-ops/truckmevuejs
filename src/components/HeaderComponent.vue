<template>
    <div class="container">
      <header>
        <div class="logo">
          <img src="../assets/logo_truck_me_frete_plataforma.webp" alt="Logo">
        </div>
  
        
        <div class="menu">
          <ul>
            <li><a href="#">Home</a></li>
          </ul>
          <ul>
            <li><a href="#">Sobre</a></li>
          </ul>
          <ul>
            <li><a href="#">Serviços</a></li>
          </ul>
          <ul>
            <li><a href="#">Contato</a></li>
          </ul>
        </div>
  
        <div class="hamburger" @click="toggleMenu">&#9776;</div>
        <nav class="menu-mobile" :class="{ show: isMenuVisible }">
          <ul>
            <li><a href="#">Home</a></li>
            <li><a href="#">Sobre</a></li>
            <li><a href="#">Serviços</a></li>
            <li><a href="#">Contato</a></li>
          </ul>
        </nav>
      </header>
    </div>
  </template>
  
  <script>
  export default {
    name: 'HeaderComponent',
    data() {
      return {
        isMenuVisible: false
      };
    },
    methods: {
      toggleMenu() {
        this.isMenuVisible = !this.isMenuVisible;
      }
    }
  };
  </script>