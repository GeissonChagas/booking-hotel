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
          <router-link to="/passeios">Passeios</router-link>
        </div>
        <div class="login">
          <router-link to="/cadastro">Cadastro</router-link>
          <router-link to="/login">Login</router-link>
        </div>
      </div>
      <div class="propagandas">
        <h1>Encontre a sua próxima estadia</h1>
        <h3>Pesquise ofertas e muito mais ...</h3>
        </div>
    </div>
</nav>

</template>

<script>
    export default{
        name:'header-component'
    }
</script>

<style scoped>
    nav {
    color: #FFF;

    }

    .banner{
    height: 350px;
    background: #003580;
    }

    .header{
    display: flex;
    justify-content: space-between;
    }

    .logo{
    padding-left: 2rem;
    }

    .services{
    display: flex;
    }

    .login{
    display: flex;
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

    nav a:hover {
    border-bottom: 2px solid #FFF;
    }

    nav a.router-link-exact-active {
    color: #FFFFFF;
    border-bottom: 2px solid #fff;
    background: rgba(255, 255, 255, 0.5);
    }

    .propagandas{
    color: #FFF;
    display: flex;
    flex-direction: column;
    justify-content: center;
    margin-top: 6rem ;
    }

    @media screen and (max-width: 768px) {
      .header{
        width: 100%;
      }
    }
</style>
