<template>
    <div class="container">
      <div class="embrulho">
        <div id="carouselExampleControls" class="carousel slide" data-bs-ride="carousel">
          <div class="carousel-inner">
            <div class="carousel-item active">
              <img src="../assets/banner.webp" class="d-block w-100" alt="...">
            </div>
            <div class="carousel-item">
              <img src="../assets/caminhao-europeu-transporta-carg.webp" class="d-block w-100" alt="...">
            </div>
            <div class="carousel-item">
              <img src="../assets/uma-linha-de-caminhoes-volvo-na.webp" class="d-block w-100" alt="...">
            </div>
          </div>
          <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleControls" data-bs-slide="prev">
            <span class="carousel-control-prev-icon" aria-hidden="true"></span>
            <span class="visually-hidden">Previous</span>
          </button>
          <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleControls" data-bs-slide="next">
            <span class="carousel-control-next-icon" aria-hidden="true"></span>
            <span class="visually-hidden">Next</span>
          </button>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'GalleryComponent',
    mounted() {
      // Certifique-se de que o carrossel está inicializado corretamente
      const bootstrap = require('bootstrap');
      const myCarousel = document.querySelector('#carouselExampleControls');
      new bootstrap.Carousel(myCarousel);
    }
  }

  </script>