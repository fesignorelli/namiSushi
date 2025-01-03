<template>
  <footer class="footer-container">
    <div class="footer-section logo-section">
      <img src="../assets/icones/logoNamiFooter.png" alt="Nami Sushi Logo" class="logo" />
      <h3>Nami Sushi</h3>
      <p class="description">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Tenetur vitae pariatur aperiam, odit quod voluptates
        cumque voluptatem? Sunt dolorem, ducimus quasi neque libero
      </p>
      <div class="newsletter">
        <input type="email" placeholder="insira seu email:" class="email-input" />
        <button class="submit-button">ENVIAR</button>
      </div>
    </div>

    <div class="footer-section menu-section">
      <h4>Menu</h4>
      <ul class="menu-list">
        <li><a href="#">Home</a></li>
        <li><a href="#">Sobre</a></li>
        <li><a href="#">Loja</a></li>
        <li><a href="#">Serviços</a></li>
        <li><a href="#">Contato</a></li>
      </ul>
    </div>

    <div class="footer-section contact-section">
      <h4>Contatos</h4>
      <ul class="contact-list">
        <li><i class="icon-location"></i> Rua Jorel da Silva, 09 - 0998-090</li>
        <li><i class="icon-email"></i> contato@petshop.com</li>
        <li><i class="icon-phone"></i> (11) 9090-9090</li> 
      </ul>
    </div>
  </footer>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'FooterComponent',
});
</script>

<style scoped>
/* Reset global */
body,
html {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  /* Garante que padding seja contabilizado no tamanho total */
}

/* Footer */
.footer-container {
  display: flex;
  justify-content: space-between;
 
  background-color: #061007;
  color: #fff;
  padding: 24px;
  width: 100%;
  height: 25rem;
  font-family: 'Arial', sans-serif;
  box-sizing: border-box;
}

.footer-section {
  display: flex;
  align-items: center;
  flex-direction: column;
  flex: 1;
}

.logo-section .logo {
  display: flex;
  justify-content: center;
  align-items: center;

  translate: 1vh 4vh; 
  width: 7vh;
}

.footer-section h3 {
  font-family: 'Times New Roman', Times, serif;
  font-size: 3vh;
}

.description {
  text-align: center;
  font-size: 2vh;
}

.newsletter {
  display: flex;
  gap: 11px;
}

.email-input {
  padding: 1vh;
  border-radius: 5px;
}

.submit-button {
  background-color: #E2462B;
  /* Vermelho */
  color: #fff;
  border: none;
  padding: 8px 16px;
  border-radius: 5px;
  cursor: pointer;
}

.submit-button:hover {
  background-color: #c0392b;
}


.menu-list{
  list-style: none;
}


.menu-list a {
  color: #fff;
}

.menu-list a:hover {
  text-decoration: underline;
}

.contact-list{
  list-style: none;
}

.footer-section h4{

  text-align: end;
}


</style>