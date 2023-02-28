<template>
  <div class="pacotes-container">
    <div class="pacotes-text">
      <h2><font-awesome-icon :icon="briefcaseIcon" />  Pacotes:</h2>
      <h1>Uma seleção de pacotes para suas próximas férias</h1>
      <p>Saindo de São Paulo</p>
    </div>
    <div class="pacotes-img">
      <div class="pacotes-card">
        <img src="https://tools-images.services.cvc.com.br/resize?width=200&height=200&url=https://almundo-com-res.cloudinary.com/image/upload/v1/CVC/destinos/nacional/RJ/RiodeJaneiro2.jpg&type=auto&quality=70" alt="">
        <h4>Rio de janeiro</h4>
        <p>Pacotes a partir de R$: <b>886,00</b></p>
      </div>
      <div class="pacotes-card">
        <img src="https://tools-images.services.cvc.com.br/resize?width=200&height=200&url=https://almundo-com-res.cloudinary.com/image/upload/v1/CVC/destinos/nacional/RS/Gramado1.jpg&type=auto&quality=70" alt="">
        <h4>Gramado</h4>
        <p>Pacotes a partir de R$: <b>1.114,00</b></p>
      </div>
      <div class="pacotes-card">
        <img src="https://tools-images.services.cvc.com.br/resize?width=200&height=200&url=https://almundo-com-res.cloudinary.com/image/upload/v1/CVC/destinos/nacional/PE/PortoGalinhas2.jpg&type=auto&quality=70" alt="">
        <h4>Porto de Galinhas</h4>
        <p>Pacotes a partir de R$: <b>1.323,00</b></p>
      </div>
    </div>
  </div>

  <div class="pacotes-container">
    <div class="pacotes-img">
      <div class="pacotes-card">
        <img src="https://tools-images.services.cvc.com.br/resize?width=200&height=200&url=https://almundo-com-res.cloudinary.com/image/upload/v1/CVC/destinos/nacional/RN/hotel/YakBeach.jpg&type=auto&quality=70" alt="">
        <h4>Natal</h4>
        <p>Pacotes a partir de R$: <b>956,00</b></p>
      </div>
      <div class="pacotes-card">
        <img src="https://tools-images.services.cvc.com.br/resize?width=200&height=200&url=https://almundo-com-res.cloudinary.com/image/upload/v1/CVC/destinos/nacional/PE/Recife2.jpg&type=auto&quality=70" alt="">
        <h4>Recife</h4>
        <p>Pacotes a partir de R$: <b>1.173,00</b></p>
      </div>
      <div class="pacotes-card">
        <img src="https://tools-images.services.cvc.com.br/resize?width=200&height=200&url=https://almundo-com-res.cloudinary.com/image/upload/v1/CVC/destinos/nacional/BA/PortoSeguro1.jpg&type=auto&quality=70" alt="">
        <h4>Porto Seguro</h4>
        <p>Pacotes a partir de R$: <b>1.082,00</b></p>
      </div>
    </div>
    <div class="pacotes-text2">
      <h2><font-awesome-icon :icon="['fas', 'plane']" />  Passagens aéreas:</h2>
      <h1>As melhores ofertas para seu voo</h1>
      <p>Saindo de São Paulo</p>
    </div>
  </div>

  <div class="pacotes-container">
    <div class="pacotes-text">
      <h2><font-awesome-icon :icon="['fas', 'hotel']" />  Hospedagens:</h2>
      <h1>Uma seleção de pacotes para suas próximas férias</h1>
      <p>Saindo de São Paulo</p>
    </div>
    <div class="pacotes-img">
      <div class="pacotes-card">
        <img src="https://tools-images.services.cvc.com.br/resize?width=200&height=200&url=https://almundo-com-res.cloudinary.com/image/upload/v1/CVC/destinos/nacional/BA/hotel/Fenix_PortoSeguro.jpg&type=auto&quality=70" alt="">
        <h4>Porto Seguro</h4>
        <p>Preços a partir de R$: <b>96,00</b></p>
      </div>
      <div class="pacotes-card">
        <img src="https://tools-images.services.cvc.com.br/resize?width=200&height=200&url=https://almundo-com-res.cloudinary.com/image/upload/v1/CVC/destinos/nacional/RJ/hotel/GamboaRioHotel.jpg&type=auto&quality=70" alt="">
        <h4>Rio de Janeiro</h4>
        <p>Preços a partir de R$: <b>114,00</b></p>
      </div>
      <div class="pacotes-card">
        <img src="https://tools-images.services.cvc.com.br/resize?width=200&height=200&url=https://almundo-com-res.cloudinary.com/image/upload/v1/CVC/destinos/nacional/RN/hotel/YakBeach.jpg&type=auto&quality=70" alt="">
        <h4>Natal</h4>
        <p>Preços a partir de R$: <b>186,00</b></p>
      </div>
    </div>
  </div>


</template>

<script>
  import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome'
  import { faBriefcase } from '@fortawesome/free-solid-svg-icons';
  
  
  export default{
    name: 'pacotes-view',
    components:{
      FontAwesomeIcon
    },
    data() {
      return {
        briefcaseIcon: faBriefcase
      }
    }
  }

</script>

<style scoped>
  .pacotes-container{
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin: 2rem auto;
    width: 90vw;
    height: 500px;
  }

  .pacotes-text{
    text-align: start;
  }
  .pacotes-text p {
    color: #777;
  }

  .pacotes-text2{
    text-align: end;
  }

  .pacotes-text2 p {
    color: #777;
  }
  .pacotes-img{
    display: flex;


  }
  .pacotes-card{
    margin: 0 0.5rem;
    box-shadow: 2px 2px 2px rgba(0,0,0, 0.1);
    padding: 1rem;
    border-radius: 5px;
    cursor: pointer;
    scale: 1.025;
    
  }
  .pacotes-card:hover{
    margin: 0 1rem;
    box-shadow: 2px 2px 4px rgba(0,0,0, 0.25);
    padding: 1rem;
    border: 1px solid #777 ;
    scale: 1.075;
    transition: 500ms;
  }
  .pacotes-card b{
    font-size: 28px;
  }

  .pacotes-card img{
    border-radius: 5px;
  }

</style>