<template>
    <footer class="footer">
      <div class="contato">
        <h4>Deixe seu e-mail e entraremos em contato:</h4>
        <div class="input-group">
          <input type="email" placeholder="Seu melhor e-mail">
          <button><font-awesome-icon :icon="['fas', 'envelope']" /></button>
        </div>
      </div>
      <div class="social-icons">
        <a href="#"><font-awesome-icon :icon="['fab', 'facebook-f']" /></a>
        <a href="#"><font-awesome-icon :icon="['fab', 'twitter']" /></a>
        <a href="#"><font-awesome-icon :icon="['fab', 'instagram']" /></a>
        <a href="#"><font-awesome-icon :icon="['fab', 'linkedin-in']" /></a>
      </div>
      <div class="copy">
        <p>Todos os direitos reservados © 2023</p>
        <p>Desenvolvido por: <a href="https://www.linkedin.com/in/geissonchagas/"> Geisson Chagas </a></p>
      </div>
    </footer>
  </template>
  
  <script>
  import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome'
  import { library } from '@fortawesome/fontawesome-svg-core'
  import { faEnvelope } from '@fortawesome/free-solid-svg-icons'
  import { faFacebookF, faTwitter, faInstagram, faLinkedinIn } from '@fortawesome/free-brands-svg-icons'
  
  library.add(faEnvelope, faFacebookF, faTwitter, faInstagram, faLinkedinIn);
  
  export default {
    name: 'FooterComponent',
    components: {
      FontAwesomeIcon
    }
  }
  </script>  
  
  <style scoped>
  .footer {
    background-color: #003580;
    color: #fff;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    height: 350px;
    margin-top: 2rem;
  }
  
  .contato {
    margin-bottom: 1rem;
  }
  
  .contato h4 {
    margin: 0;
  }
  
  .input-group {
    display: flex;
    align-items: center;
    margin-top: 0.5rem;
  }
  
  .input-group input {
    width: 30vw;
    height: 30px;
    margin-right: 0.5rem;
    padding: 5px;
    border: none;
    border-radius: 5px;
  }
  
  .input-group button {
    background-color: transparent;
    border: none;
    color: #fff;
    font-size: 1.5rem;
    cursor: pointer;
    scale: 1.5;
  }
  
  .input-group button:hover {
    color: #3872c4;
    scale: 1.75;
  }
  
  .social-icons {
    display: flex;
    justify-content: center;
  }
  
  .social-icons a {
    color: #fff;
    font-size: 1.5rem;
    margin: 0 0.5rem;
  }
  
  .copy {
    text-align: center;
    margin-top: 1rem;
  }
  
  .copy p {
    margin: 0;
  }
  
  .copy a {
    color: #fff;
  }

  .copy font-awesome-icon{
    background: #3872c4;
  } 
  </style>
  