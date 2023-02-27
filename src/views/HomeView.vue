<template>
 <div>
    <div class="carousel">
      <CarouselComponent />
    </div>
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

    <div class="descubra-br">
      <h2>Descubra no Brasil</h2>
      <ul class="cards-container">
        <li class="cards-descubra">
          <img
            src="https://q-xx.bstatic.com/xdata/images/city/250x250/653641.jpg?k=29b8706ee4bff7b870ca35a698c5ac4be003b4122b00035a9d4a572d3101b1fe&o="
            alt="imagem rj"
          />
          <h4>Local</h4>
          <p>600 alojamentos</p>
        </li>
        <li class="cards-descubra">
          <img
            src="https://q-xx.bstatic.com/xdata/images/city/250x250/653646.jpg?k=0a8eb3999748f5b12b29f6bd5492a12b7f15a37535e572ea91403098d1588d38&o="
            alt="imagem sp"
          />
          <h4>São Paulo</h4>
          <p>500 alojamentos</p>
        </li>
        <li class="cards-descubra">
          <img
            src="https://q-xx.bstatic.com/xdata/images/city/250x250/349399.jpg?k=6f023ae905561a547be6cc5cb117571b4a1425b633e767cdbbf797bb5225dd18&o="
            alt="imagem gramado"
          />
          <h4>Gramado</h4>
          <p>390 alojamentos</p>
        </li>
        <li class="cards-descubra">
          <img
            src="https://q-xx.bstatic.com/xdata/images/city/250x250/653621.jpg?k=7d0330a52ee7350d5d38c6cbdf7349f4798889706117e38e74f04e631e09b31b&o="
            alt="imagem gramado"
          />
          <h4>Porto de Galinhas</h4>
          <p>200 alojamentos</p>
        </li>
      </ul>
    </div>


  <div class="descubra-alojamentos">
    <h2>Escolha o onde se hospedar</h2>

      <ul class="alojamentos-container">
        <li class="cards-alojamentos">
          <img
            src="https://th.bing.com/th/id/R.0c3606845a94351e6b7354ed4f6561fb?rik=PCkkyIQ%2fYDc1xQ&pid=ImgRaw&r=0"
            alt="imagem hotel"
          />
          <h4>Hoteis</h4>
          <p>600 opções</p>
        </li>
        <li class="cards-alojamentos">
          <img
            src="https://th.bing.com/th/id/R.9172d20fccd2103cb641d25496ff00ba?rik=I0Ulpev8GtMbLQ&riu=http%3a%2f%2fst.gde-fon.com%2fwallpapers_original%2f367049_pejzazh_priroda_domik_voda_otrazhenie_1680x1050_www.Gde-Fon.com.jpg&ehk=ItbyDkI32Sdvo%2fzhtk5vwnyyhE6pEY6RnuDgBjlZ1to%3d&risl=&pid=ImgRaw&r=0"
            alt="imagem pousada"
          />
          <h4>Pousadas</h4>
          <p>600 opções</p>
        </li>
        <li class="cards-alojamentos">
          <img
            src="https://images7.alphacoders.com/345/345182.jpg"
            alt="imagem resort"
          />
          <h4>Resorts</h4>
          <p>600 opções</p>
        </li>
        <li class="cards-alojamentos">
          <img
            src="https://p4.wallpaperbetter.com/wallpaper/773/841/74/architecture-building-design-house-wallpaper-preview.jpg"
            alt="imagem casa"
          />
          <h4>Casas</h4>
          <p>600 opções</p>
        </li>
      </ul> 
  </div>

</template>

<script>
import FormularioPesquisa from "../components/FormularioPesquisa.vue";
import CarouselComponent from "@/components/CarouselComponent.vue";


export default {
  name: "pacotes-view",
  components: {
    FormularioPesquisa,
    CarouselComponent

  },
};
</script>

<style scooped>

.carousel img{
  width: 100vw;
  max-width: 1980px;
  height: 550px;
}
.promocoes {
  display: flex;
  justify-content: space-around;
  margin: 1rem auto 0 auto;
  flex-wrap: wrap;
  height: 220px;
  max-width: 80vw;
}

.promocoes-card{
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: center;
  background-image: url(https://q-xx.bstatic.com/xdata/images/xphoto/714x300/182431478.jpeg?k=fcbb6d5552a1d4ff338978206c449077ab8ad696050cfd7e4edef1ddc11225cc&o=);
  background-size: cover;
  color: #fff;
  width: 470px;
  box-shadow: 2px 2px 4px 4px rgba(0, 0, 0, 0.5);
  margin-top: 2rem;
}

.promocoes-card2 {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: center;
  background-image: url(https://th.bing.com/th/id/OIP.Gaz_TpDGA00kwN7TWL9sUQHaFj?pid=ImgDet&w=1024&h=768&rs=1);
  background-size: cover;
  color: #fff;
  width: 470px;
  box-shadow: 2px 2px 4px 4px rgba(0, 0, 0, 0.5);
  margin-top: 2rem;
}

button {
  width: 100px;
  height: 35px;
  font-weight: 700;
  color: #fff;
  background: #008cf0;
  border: none;
  border-radius: 3px;
  cursor: pointer;
  display: flex;
  align-items: center;
  justify-content: center;
  margin: 0.25rem auto;
}

button:hover {
  background: #003580;
  transition: 300ms;
  scale: 1.025;
}

.cards-container {
  display: flex;
  justify-content: space-between;
  margin: 1rem auto;
  flex-wrap: wrap;
  max-width: 80vw;
}

.descubra-br {
  background: #f6f6f6;
  text-align: center;
  margin: 2rem 0;
}

.cards-descubra {
  display: flex;
  flex-direction: column;
  width: 12.5rem;
  margin: 0 1rem;

}

.alojamentos-container{
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
  width: 80vw;
  margin: 0 auto;
}

.cards-descubra img {
  width: 12rem;
  width: 12rem;
  border-radius: 5px;
}

.cards-descubra p {
  color: #555;
  font-size: 12px;
  margin: 0 auto;
}

.cards-descubra h4{
  margin: 0.5rem auto 0 auto;
}

.cards-alojamentos{
    margin: 0 auto;
  }

.cards-alojamentos img{
  width: 25rem;
  height: 15rem;
  border-radius: 8px;
}


@media screen and (min-width: 1450px) {
  .cards-alojamentos img{
    width: 18rem;
    height: 10rem;
  }
}
@media screen and (max-width: 768px) {
  .promocoes{
    width: 100vw;
  }
  .promocoes-card, .promocoes-card2{
    margin: 1rem auto;
  }

  .descubra-br{
    margin: 10rem auto;
  }

  @media screen and (max-width: 414px;) {
    .carousel img{
      height: 300px;
    }
    
  }

}
</style>