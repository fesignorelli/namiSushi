<template>
  <nav class="navbar">
    <!-- Logo -->
    <div class="logo">
      <img src="../assets//icones/logoNamiSushi.png" alt="Logo" class="logo-img" />
    </div>

    <!-- Botão do menu hambúrguer -->
    <button class="hamburger" @click="toggleMenu">
      <span></span>
      <span></span>
      <span></span>
    </button>

    <!-- Links de navegação -->
    <ul :class="['nav-links', { open: isMenuOpen }]">
      <li><a href="#">Home</a></li>
      <li><a href="#">About Us</a></li>
      <li><a href="#">Cardápio</a></li>
    </ul>

    <!-- Ícones -->
    <div class="nav-icons">
      <a href="#"><i class="fas fa-search"></i></a>
      <a href="#"><i class="fas fa-shopping-cart"></i></a>
      <a href="#"><i class="fas fa-user"></i></a>
    </div>
  </nav>
</template>

<script lang="ts">
import { defineComponent, ref } from 'vue';

export default defineComponent({
  name: 'Navbar',
  setup() {
    const isMenuOpen = ref(false);

    const toggleMenu = () => {
      isMenuOpen.value = !isMenuOpen.value;
    };

    return {
      isMenuOpen,
      toggleMenu,
    };
  },
});
</script>

<style scoped>
/* Reset básico */
body {
  margin: 0;
  padding: 0;
  font-family: 'Arial', sans-serif;
}

.navbar {
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 10px 50px;
}

.logo {
  display: flex;
  justify-content: center;
  align-items: left;
  translate: -60vh;
}

.logo-img {
  height: 5rem;
}

.nav-links {
  display: flex;
  list-style: none;
  gap: 10vh;
}

.nav-links li a {
  text-decoration: none;
  color: #000;
  font-size: 2.5vh;
  font-weight: bold;
  font-family: 'Times New Roman', Times, serif;
}

.nav-links li a:hover {
  color: #8b8b56;
}

.nav-icons {
  display: flex;
  gap: 15px;
}

.nav-icons a {
  color: #000;
  font-size: 20px;
  text-decoration: none;
}

.nav-icons a:hover {
  color: #8b8b56;
}

/* Estilo do menu hambúrguer */
.hamburger {
  display: none;
  flex-direction: column;
  gap: 5px;
  background: none;
  border: none;
  cursor: pointer;
}

.hamburger span {
  width: 25px;
  height: 3px;
  background-color: #000;
  border-radius: 2px;
  transition: all 0.3s ease-in-out;
}

/* Responsividade */
@media (max-width: 768px) {
  .nav-links {
    display: none;
    flex-direction: column;
    position: absolute;
    top: 60px;
    right: 20px;
    background-color: #fff;
    padding: 10px;
    border-radius: 5px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    z-index: 10;
  }

  .nav-links.open {
    display: flex;
  }

  .hamburger {
    display: flex;
  }

  .nav-icons {
    gap: 10px;
  }
}

@media (max-width: 480px) {

  .hamburger {
    display: flex;
    translate: 20rem;
  }
}
</style>
