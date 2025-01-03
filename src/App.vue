<script lang="ts">
import Banner from './components/Banner.vue';
import MenuCards from './components/MenuCards.vue';
import Tradicao from './components/Tradicao.vue';
import Testemunha from './components/Testemunha.vue';
import FooterNami from './components/FooterNami.vue';
import Navbar from './components/Navbar.vue';

export default {
  components: { Banner, Tradicao, MenuCards, Testemunha, FooterNami, Navbar }
}

</script>

<template>
  <Navbar />
  <Banner />
  <Tradicao />
  <MenuCards />
  <Testemunha />
  <FooterNami />
</template>