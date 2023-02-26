<template>

  <HeaderComponent />
  <router-view/>
  <FooterComponent />

</template>

<script>
  import HeaderComponent from './components/HeaderComponent.vue'
  import FooterComponent from './components/FooterComponent.vue';

  export default{
    name: 'App',
    components: {
      HeaderComponent,
      FooterComponent

    }
  }
</script>

<style>
#app {
  font-family: 'Montserrat', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  width: 100vw;
  margin: 0;
  padding: 0;
  
  
}
:placeholder-shown, ::placeholder, input, button, a {
  font-family: 'Montserrat', sans-serif;
}

li{
  list-style: none;
}

a{
  text-decoration: none;
}

body {
  overflow-x: hidden;
}


</style>

