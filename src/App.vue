<template>
  <nav>
    <div class="banner">
      <div class="header">
        <div class="logo">
          <h4>BookHotels</h4>
        </div>
        <div class="services">
          <router-link to="/">Início</router-link>
          <router-link to="/pacotes">Pacotes</router-link>
          <router-link to="/voos">Voos</router-link>
          <router-link to="/translado">Translado</router-link>
        </div>
        <div class="login">
          <router-link to="/cadastro">Cadastre-se</router-link>
          <router-link to="/login">Login</router-link>
        </div>
      </div>
    </div>
  </nav>

  <router-view/>
</template>

<style>
#app {
  font-family: 'Montserrat', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  width: 100vw;
  
}

nav {
  color: #FFF;

}

.banner{
  display: flex;
  align-items: center;
  height: 350px;
  background: #003580;
}

nav a {
  display: flex;
  justify-content: space-around;
  flex-direction: row;
  font-weight: bold;
  color: #FFFFFF;
  text-decoration: none;
  padding: 1rem;
  margin: 0 1rem;
}

nav a.router-link-exact-active {
  color: #FFFFFF;

  background: rgba(255, 255, 255, 0.5);
}
</style>
