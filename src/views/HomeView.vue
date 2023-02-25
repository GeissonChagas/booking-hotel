<template>

  <div>
    <h2>Faça aqui sua pesquisa:</h2>
    <FormularioPesquisa />
  </div>

  <div class="promocoes">
    <div class="promocoes-card">
      <h4>Conheça lugares novos com nossos pacotes</h4>
      <p>Oportunidades nacionais e internacionais</p>
      <button>Saiba mais</button>
    </div>
    <div class="promocoes-card2">
      <h4>Aproveite o verão no litoral</h4>
      <p>Pacotes promocionais para praias em todo Brasil</p>
      <button>Saiba mais</button>
    </div>
  </div>


</template>

<script>

import FormularioPesquisa from '../components/FormularioPesquisa.vue'

  export default{
    name: 'pacotes-view',
    components: {
      FormularioPesquisa
    }
  }

</script>

<style scooped>

  .promocoes{
    display: flex;
    justify-content: space-around;
    height: 220px;
    width: 100vw;
    margin-top: 1rem;
  }

  .promocoes-card{
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    align-items: center;
    background-image: url(https://q-xx.bstatic.com/xdata/images/xphoto/714x300/182431478.jpeg?k=fcbb6d5552a1d4ff338978206c449077ab8ad696050cfd7e4edef1ddc11225cc&o=);
    background-size: cover;
    color: #FFF;
    width: 470px;
    box-shadow: 2px 2px 4px 4px rgba(0, 0, 0, 0.5);
  }

  .promocoes-card2{
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    align-items: center;
    background-image: url(https://th.bing.com/th/id/OIP.Gaz_TpDGA00kwN7TWL9sUQHaFj?pid=ImgDet&w=1024&h=768&rs=1);
    background-size: cover;
    color: #FFF;
    width: 470px;
    box-shadow: 2px 2px 4px 4px rgba(0, 0, 0, 0.5);
  }

  button{
    width: 100px;
    height: 30px;
    font-weight: 700;
    color: #FFF;
    background: #008cf0;
    border: none;
    border-radius: 5px ;
    cursor: pointer;
  }





</style>
