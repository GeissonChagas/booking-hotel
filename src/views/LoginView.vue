<template>
  <div class="login-container">
    <form @submit.prevent="login">
      <h2>Login</h2>
      <div class="form-group">
        <label for="email">E-mail:</label>
        <input type="email" id="email" class="form-input" v-model="email" required />
      </div>
      <div class="form-group">
        <label for="senha">Senha:</label>
        <input type="password" id="senha" class="form-input" v-model="senha" required />
      </div>
      <button type="submit" class="form-submit">Entrar</button>
    </form>
  </div>
</template>

<script>
export default {
  data() {
    return {
      email: '',
      senha: ''
    }
  },
  methods: {
    login() {
      // Lógica de autenticação do usuário
    }
  }
}
</script>

<style>

.login-container {
  margin: 5rem auto;
  max-width: 80%;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
  padding: 20px;
  border-radius: 10px;
  display: flex;
  justify-content: center;
  align-items: center;
}

.login-container form{
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
