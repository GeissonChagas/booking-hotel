<template>
  <nav>
    <div class="banner">
      <div class="header">
        <div class="logo">
          <h4>BookHotels</h4>
          <font-awesome-icon :icon="['fas', 'plane']" />
        </div>
        <div class="menu-icon" @click="toggleMenu">
          <i class="fas fa-bars"></i>
        </div>
        <div class="close-icon" @click="closeMenu" v-show="showMenu">
          <i class="fas fa-times"></i>
        </div>
        <div class="menu" :class="{ 'show-menu': showMenu }">
          <router-link to="/">Início</router-link>
          <router-link to="/pacotes">Pacotes</router-link>
          <router-link to="/voos">Voos</router-link>
          <router-link to="/passeios">Passeios</router-link>
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
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome';
export default {
  name: "header-component",
  components: {
    FontAwesomeIcon
  },
  data() {
    return {
      showMenu: false,
    };
  },
  methods: {
    toggleMenu() {
      this.showMenu = !this.showMenu;
    },
    closeMenu() {
      this.showMenu = false;
    },
  },
};
</script>

<style scoped>
nav {
  color: #fff;
  overflow-x: hidden;
}

.banner {
  height: 350px;
  background: #003580;
  max-width: 100vw;
}

.header {
  display: flex;
  justify-content: space-between;
}

.logo {
  display: flex;
  align-items: center;
  padding: 0 2rem;
}

.logo h4{
  margin-right: 1rem;
}

.logo i.fas.fa-plane {
  margin-left: 5px;
}


.menu-icon {
  display: none;
  font-size: 1.5rem;
  padding-right: 2rem;
  cursor: pointer;
  margin-left: 2rem;
}

a{
  color: #fff;
  text-decoration: none;
  margin: 0 1rem;
  padding: 1rem;
}

a:hover{
  border-bottom: 2px solid #FFF;
  background-color: rgba(255,255,255, 0.5);
  transition:500ms;
  
}
.menu {
  display: flex;
  flex-direction: row;
  align-items: center;
}

.menu.show-menu {
  display: flex;
  flex-direction: column;
  position: fixed;
  top: 0;
  right: 0;
  width: 60%;
  max-width: 70vw;
  height: 100%;
  background: #003580;
  
}


.menu.show-menu a:hover {
  background: rgba(255,255,255, 0.5);
  color: #003580;
}

.menu.show-menu a.router-link-exact-active {
  background: rgba(255,255,255, 0.5);
  color: #003580;
}

.propagandas {
  color: #fff;
  display: flex;
  flex-direction: column;
  justify-content: center;
  margin-top: 6rem;
}

.close-icon {
  display: none;
    font-size: 18px;
    padding-right: 2rem;
    cursor: pointer;
    position: absolute;
    top: 1rem;
    right: 15rem;
    z-index: 1;
    scale: 1.25;
    
}

@media screen and (max-width: 768px) {
  .header {
    flex-direction: column;
    align-items: flex-start;
  }

  .logo {
    display: none;
  }
  .menu-icon {
    display: block;
    margin: 1rem;
  }
  .close-icon {
    display: block;
  }
  .menu {
    display: none;
  }
  .menu.show-menu {
    display: flex;
    flex-direction: column;
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    background: #3b7edb;
  }
}
</style>

