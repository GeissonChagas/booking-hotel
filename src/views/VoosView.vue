<template>
    <div class="banner-voos">
      <h2>Para onde vamos?</h2>
    </div>
    <div>
      <FormularioPesquisa />
    </div>
    <div>
      <div>
        <h2>Cidades populares:</h2>
        <div class="cards-container">
          <div class="cards-voos">
            <img src="https://q-xx.bstatic.com/xdata/images/city/square210/653487.jpg?k=1d56a1c05cf750713aec2eef45b0f4eb5feea777e9e94cf3b9d0956f0286a9ec&o=" alt="">
            <h4>Foz do Iguaçu</h4>
            <p>Saída xx/xx/xx</p>
          </div>
          <div class="cards-voos">
            <img src="https://q-xx.bstatic.com/xdata/images/city/square210/971982.jpg?k=b65c557258d14ccaf06765683a26d8f2bc5088d751af34e0986923daa72eab98&o=" alt="">
            <h4>Porto, Portugal</h4>
            <p>Saída xx/xx/xx</p>
          </div>
          <div class="cards-voos">
            <img src="https://q-xx.bstatic.com/xdata/images/city/square210/619964.jpg?k=7e2df42a96dbbc8ccb8fa9446e4b63cf7bebe4123a41e387314ce3538eea0df7&o=" alt="">
            <h4>Lisboa, Portugal</h4>
            <p>Saída xx/xx/xx</p>
          </div>
          <div class="cards-voos">
            <img src="https://q-xx.bstatic.com/xdata/images/city/square210/653645.jpg?k=f54715ae6012a3f9481faedab3bc8a07549a24b964a14565e1f5b79338418166&o=" alt="">
            <h4>São Paulo, BR</h4>
            <p>Saída xx/xx/xx</p>
          </div>
          
        </div>
      </div>
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

    .cards-container{
      background: #f2f2f2;
      width: 100vw;
      margin: 0 auto;
      padding: 1rem;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.2)
    }


    .cards-voos{
      border: 1px solid rgba(0,0,0, 0.1);
      padding: 1rem;
      border-radius: 5px;
      margin: 0 auto;
    }




  
  
  </style>