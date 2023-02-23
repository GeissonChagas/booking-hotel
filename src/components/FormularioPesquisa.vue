<template>
    <div class="formulario-pesquisa">
      <form>
        <div class="input-container">
          <label for="destination">Destino:</label>
          <input type="text" id="destination" v-model="destination" placeholder="Para onde você quer ir?" />
        </div>
        <div class="input-container">
          <label for="checkin">Check-in:</label>
          <input type="date" id="checkin" v-model="checkin" />
        </div>
        <div class="input-container">
          <label for="checkout">Check-out:</label>
          <input type="date" id="checkout" v-model="checkout" />
        </div>
        <div class="input-container">
          <label for="guests">Hóspedes:</label>
          <input type="number" id="guests" v-model="guests" />
        </div>
        <button type="submit">Buscar</button>
      </form>
    </div>
  </template>
  
  <script>
  export default {
    name: 'formulario-pesquisa',
    data() {
      return {
        destination: '',
        checkin: '',
        checkout: '',
        guests: 1
      }
    }
  }
  </script>
  
  <style scoped>
    .formulario-pesquisa {
        background-color: #f6f6f6;
        padding: 20px;
        border-radius: 4px;
    }
    .formulario-pesquisa form{
        display: flex;
        justify-content: center;
        align-items: center;
    }
    .input-container {
        display: flex;
    }
    label {
        font-weight: bold;
        display: flex;
        align-items: center;
        margin: 0 1rem;
    }
    input {
        padding: 10px;
        border-radius: 4px;
        border: none;
        background-color: #fff;
        box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
    }
    button {
        background-color: #008cf0;
        color: #fff;
        border: none;
        border-radius: 4px;
        padding: 10px;
        cursor: pointer;
        font-weight: 700;
    }
    button:hover {
        background-color:#00487a;
        transition: 500ms;
    }
  </style>
  