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
      <div class="button-container">
        <button type="submit">Buscar</button>
      </div>
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
  display: flex;
  justify-content: center;
}
.formulario-pesquisa form {
  background-color: #f6f6f6;
  padding: 20px;
  border-radius: 4px;
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 80%;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
}


.input-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-bottom: 20px;
  width: 100%;
}

label {
  font-weight: bold;
  margin-bottom: 10px;
}

input {
  padding: 10px;
  border-radius: 4px;
  border: none;
  background-color: #fff;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
  width: 100%;
  max-width: 400px;
}

.button-container {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100%;
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
  background-color: #00487a;
  transition: 500ms;
}
</style>
