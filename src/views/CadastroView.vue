<template>
  <div class="cadastro-container">
    <form @submit.prevent="cadastrar">
      <h2>Cadastro</h2>
      <div class="form-group">
        <label for="nome">Nome:</label>
        <input type="text" id="nome" class="form-input" v-model="nome" required />
      </div>
      <div class="form-group">
        <label for="email">E-mail:</label>
        <input type="email" id="email" class="form-input" v-model="email" required />
      </div>
      <div class="form-group">
        <label for="senha">Senha:</label>
        <input type="password" id="senha" class="form-input" v-model="senha" required />
      </div>
      <div class="form-group">
        <label for="confirmarSenha">Confirmar senha:</label>
        <input type="password" id="confirmarSenha" class="form-input" v-model="confirmarSenha" required />
      </div>
      <button type="submit" class="form-submit">Cadastrar</button>
    </form>
  </div>
</template>

<script>
export default {
  data() {
    return {
      nome: '',
      email: '',
      senha: '',
      confirmarSenha: ''
    }
  }
}
</script>

<style>

.cadastro-container {
  margin: 5rem auto;
  max-width: 80%;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
  padding: 20px;
  border-radius: 10px;
  display: flex;
  justify-content: center;
  align-items: center;
}

.cadastro-container form{
  width: 100%;
}

.form-group {
  margin-bottom: 20px;
}

label {
  display: inline-block;
  width: 50%;
  align-items: center;
  font-weight: bold;
  margin-right: 10px;
  margin-bottom: 5px;
}

input[type="text"],
input[type="email"],
input[type="password"] {
  display: flex;
  align-items: center;
  width: 60%; 
  margin: 0 auto;
  padding: 10px;
  border: 1px solid #ccc;
  border-radius: 5px;
  box-shadow: 0 0 5px rgba(0, 0, 0, 0.2);
}



button[type="submit"] {
  background-color: #0369f8;
  color: white;
  padding: 10px 20px;
  border: none;
  border-radius: 5px;
  cursor: pointer;
}

button[type="submit"]:hover {
  background-color: #003580;
}

</style>
