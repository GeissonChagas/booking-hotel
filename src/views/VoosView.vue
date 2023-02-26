<template>
    <div class="banner-voos">
      <h2>Para onde vamos?</h2>
    </div>
    <div>
      <FormularioPesquisa />
    </div>
  
  </template>
  
  <script>

  import FormularioPesquisa from '@/components/FormularioPesquisa.vue';


    export default{
      name: 'voos-view',
      components: {
        FormularioPesquisa
      }
    }
  
  </script>
  
  <style>
    .banner-voos {
      background-image: url(https://th.bing.com/th/id/R.1569bde6fa13a40de351b92adbccde39?rik=7FUOCBZEbOnLgA&pid=ImgRaw&r=0);
      background-size: cover;
      height: 500px;
      width: 100%;
      background-position: center;
      background-repeat: no-repeat;
      color: #555;
      margin: 0 auto 2rem auto;
      box-shadow: 0px -10px 20px 10px rgba(255, 255, 255, 0.5);
    }

    .banner-voos h2 {
      background: rgba(255,255,255,0.5);
      display: inline-block;
    }




  
  
  </style>