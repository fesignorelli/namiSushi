<template>
  <div class="menu-container">
    <h1 class="titulo-menu-container">
      Conheça alguns dos nossos pratos!
    </h1>

    <div class="menu-grid">
      <div class="menu-item" v-for="item in menuItems" :key="item.title">
        <img :src="item.image" :alt="item.title" class="item-image" />
        <h3>{{ item.title }}</h3>
        <p>{{ item.description }}</p>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import SushiSashimi from '../assets/imagens/sushisPedido.png';
import PorcaoDeSushi from '../assets/imagens/sushiPedido.png';
import ChurrascoNaTabua from '../assets/imagens/churrascoPedido.png';

interface MenuItem {
  title: string;
  description: string;
  image: string;
}

export default defineComponent({
  name: "Menu",
  data() {
    return {
      menuItems: [
        {
          title: "Sushi e Sashimi",
          description:
            "Sashimi, peixe cru fatiado finamente e diversos recheios nos sushis.",
          image: PorcaoDeSushi,
        },
        {
          title: "Porção de Sushi",
          description: "Uma viagem gastronômica pelo Japão em cada garfada.",
          image: SushiSashimi,
        },
        {
          title: "Churrasco na Tábua",
          description: "Carne suculenta com um toque oriental.",
          image: ChurrascoNaTabua,
        },
      ] as MenuItem[],
    };
  },
});
</script>

<style scoped>

.titulo-menu-container {
  font-family: 'Times New Roman', Times, serif;
  color: #000;
  font-size: 3rem;
  width: 100%; /* Ajuste para ocupar toda a largura */
  text-align: center; /* Centraliza o texto */
}

.menu-container {
  
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  padding: 10vh 2vw; /* Melhora o espaçamento para telas menores */
  font-family: Arial, sans-serif;
  font-size: 3vh; /* Ajuste proporcional ao layout */
  text-align: center;
}

.menu-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); /* Melhor controle do tamanho mínimo */
  width: 100%;
  max-width: 1200px; /* Maior limite para telas grandes */
}

.menu-item {
font-family: 'Times New Roman', Times, serif;

  display: flex; /* Alinha itens internos */
  flex-direction: column;
  justify-content: center;
  align-items: center;

  text-align: center;
  background-color: #3c5f34;
  padding: 1rem;
  width: 80%; /* Remove o valor fixo para melhor responsividade */
  height: 100%; /* Ajuste para ser dinâmico */
  border-radius: 10px;
  color: #fff;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2); /* Suaviza o sombreado */
  transition: transform 0.3s, box-shadow 0.3s; /* Animações suaves */
}

.menu-item:hover {
  transform: scale(1.05); /* Efeito de zoom ao passar o mouse */
  box-shadow: 0 6px 12px rgba(0, 0, 0, 0.3); /* Destaque maior ao passar o mouse */
}

.item-image {
  display: flex;
  justify-content: center;
  align-items: center; /* Certifica-se de centralizar a imagem */
  width: 60%;
}

</style>