<template>
<div>
  <HeaderComponent/>
  <BannerComponent/>
  <AboutComponent/>
  <SaibaMaisComponent/>
  <ServicesTableComponent/>
  <ContactFormComponent/>
  <GalleryComponent/>
  <ComponentRodaPe/>
</div>
</template>

<script>
  
  import HeaderComponent from './components/HeaderComponent.vue';
  import BannerComponent from './components/BannerComponent.vue';
  import AboutComponent from './components/AboutComponent.vue';
  import SaibaMaisComponent from './components/SaibaMaisComponent.vue';
  import ServicesTableComponent from './components/ServicesTableComponent.vue';
  import ContactFormComponent from './components/ContactFormComponent.vue';
  import GalleryComponent from './components/GalleryComponent.vue';
  import ComponentRodaPe from './components/ComponentRodaPe.vue';


  export default {
    name: 'App',

    components: {
      HeaderComponent,
      BannerComponent,
      AboutComponent,
      SaibaMaisComponent,
      ServicesTableComponent,
      ContactFormComponent,
      GalleryComponent,
      ComponentRodaPe
    } 
  }

  

</script>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,100;0,300;0,400;0,500;0,700;0,900;1,100;1,300;1,400;1,500;1,700;1,900&display=swap');

*{

    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: "Roboto", sans-serif;
}

.container{
    max-width: 1280px;
    margin: 0 auto;
    
}

.logo img{
    width: 200px;
    margin: 10px;
}

.menu{
    display: inline-flex;
    
}

menu i{
        display: none;
        font-size: 30px;
        cursor: pointer;
        color: #f05123;
}

header{
    display: flex;
    justify-content: space-between;
    padding: 10px;
    flex-wrap: wrap;
}


ul li{
    list-style-type: none;
    padding-right: 18px;
    margin-top: 20px;
    
}

ul li a{
   
    text-decoration: none;
    font-size: 18px;
    font-weight: bold;
    text-transform: uppercase;
    color: #f05123;
}   

a:hover{
    color: black;
}

.banner{
    height: 90vh;
    width: 100%;
    text-align: center;

}

.bannerimg {
    max-height: 100%;
    height: 90vh;
    width: 100%;
    background-image: url('./assets/banner.webp');
    background-size: cover;
    background-position: center;
    position: relative;
}


.title-banner{
    text-align: center;
    position: absolute;
    z-index: 10;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    color: aliceblue;
    font-size: 80px;
    background-color: hsla(13, 87%, 54%, 0.5);
    text-shadow: 0px 6px 11px rgba(0, 0, 0, 0.69);
}

.sobre{
    margin-top: 20px;
    margin-bottom: 20px;
}

h2{
    text-align: center;
    color: #F05123;
    font-size: 45px;
    padding: 20px;
    text-transform: uppercase;
}

 .sobre p{
    padding: 0 2%;
    text-align: center;
    font-size: 18px;
    line-height: 20px;
    margin-top: 20px;
 }

 .sobre{
    text-align: center;
 }

 .sobre button{
    margin-top: 40px;
 }

.sobre i{
    margin-left: 20px ;
 }

 .nossos-servicos{
    background-color: #F05123;
    padding: 20px;
 }

.nossos-servicos h2{
    text-align: center;
    color: #ffffff;
    font-size: 45px;
    padding: 20px;
    text-transform: uppercase;
 }

 .container-servicos{
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    
 }

 .single{
    padding: 10px;
    width: 500px;
    border: 1px solid #862e16;
    margin:20px;
    text-align: center;
    border-radius: 20px;
 }

 .single i{
    font-size: 35px;
    padding: 12px;

 }

 .single p{
    color:white;
    font-weight: lighter;
    font-size: 20px;
 }

.single h2{
    font-weight: bold;
    margin-top: 8px;
    font-size: 22px;
 }

 .single h3{
    color: #ffffff;
    font-size: 20px;
    padding: 5px;
 }

.formulario {
    margin: 0 auto;
    width: 350px;
}

form{
    text-align: center;
    padding: 20px;
 
}

.email, 
.name{
    margin-top: 20px;
    width: 100%;
    height: 30px;
    border-radius: 10px;
    border: 1px solid #f05123;
    padding: 8px;
    
}
 .mensagem{
    margin-top: 20px;
    width: 100%;
    height: 120px;
    border-radius: 10px;
    border: 1px solid #f05123;
    padding: 8px;
}

.envia,
.saiba{
    margin-top: 20px;
    padding: 10px;
    background-color: #f05123;
    border: none;
    font-size: 20px;
    color: white;
    width: 200px;
    border-radius: 20px;
    cursor: pointer;
}

footer{
    margin-top: 60px;
    justify-content: space-between;
    display: flex;
    background-color: #ffe7e0;
    text-align: center;
    padding: 30px;
}

footer h4{
    font-size: 16px;
}

footer img{
    width: 120px;

}

/*Interativos*/

.hamburger {
    display: none;
    font-size: 30px;
    cursor: pointer;
    color: rgb(0, 0, 0);
}

.menu-mobile {
    display: none;
    flex-direction: column;
    background-color: #f05123;
    position: absolute;
    top: 80px;
    right: 0;
    width: 100%;
    text-align: center;
}

.menu-mobile ul {
    list-style: none;
    padding: 0;
}

.menu-mobile ul li {
    padding: 10px 0;
}

.menu-mobile ul li a {
    color: white;
    text-decoration: none;
    font-size: 18px;
    font-weight: bold;
}


.saiba-mais-text{
    text-align: center;
    padding: 40px ;
    border: 2px dotted coral;
    margin: 16px;
}

.saiba-mais-text p{
    margin: 20px;
    font-size: 18px;
}


.saiba-mais {
    
    max-height: 0;
    overflow: hidden;
    opacity: 0;
    transition: max-height 1s ease-out, opacity 1s ease-out;
}

.saiba-mais.show {
    max-height: 1000px; 
    opacity: 1;
    transition: max-height 1s ease-in, opacity 1s ease-in;
    
}

.embrulho{
    margin: 50px auto;
    width: 100%;
}


.carousel-item img {
    height: 100%;
    width: 100%;
    object-fit: cover; /* Ajusta as imagens para se conterem dentro do contêiner */
}

.carousel-control-prev-icon,
.carousel-control-next-icon {
    background-color: #f05123; /* Altere esta cor conforme necessário */
    width: 50px;
    height: 50px;
    background-size: 100%, 100%;
    border-radius: 30%;
}


@media screen and (max-width: 680px) {

    .menu{
        display: none;
    }

    .hamburger {
        display: block;
    }

    .menu-mobile.show {
        display: flex;
        z-index: 999;
    }

    .menu-mobile.show a:hover{
        color: black;
        border-bottom: 2px solid black;
    }
    

    footer{
        display: block;
    }

    footer .logo-footer{
        margin-top: 10px;
    }
    

}




</style>
