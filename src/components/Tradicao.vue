<template>
  <div class="tradicao-section">
    <div class="overlay">
      <h1>"Sabor que Encanta, Tradição que Inspira"</h1>
      <p>
        A tradição é a alma do Nami Sushi. Cada prato é uma homenagem à rica herança culinária do Japão,
        onde técnicas ancestrais são mantidas e respeitadas. Desde o preparo meticuloso do sushi até a
        apresentação cuidadosa dos pratos, honramos os métodos clássicos que têm sido transmitidos de
        geração em geração. Acreditamos que, ao preservar essas tradições, oferecemos uma experiência
        autêntica e enriquecedora a nossos clientes.
      </p>
    </div>
  </div>
</template>

<style scoped>
.tradicao-section {
  margin-top: 20%;
  background-image: url('../assets/imagens/restauranteFundo.png');
  /* Substitua pelo caminho da imagem */
  background-size: 100% 100%;

  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
}


.overlay {
  display: block;
  justify-content: center;
  text-align: center;
  align-items: center;



  background-color: rgba(23, 60, 28, 0.8);
  /* Fundo escuro com transparência */
  color: white;
  padding: 30vh;
}

h1 {
  font-family: 'Times New Roman', Times, serif;
  justify-content: center;
  display: flex;
  align-items: center;

  text-align: center;
  font-size: 3rem;
  font-weight: bold;
}

p {
  justify-content: center;
  display: flex;
  align-items: center;

  margin: 0 auto;
  text-align: center;
  width: 100%;
  font-weight: 400;
  font-size: 3vh;
}

@media (max-width: 768px) {
  h1 {
    font-size: 1.5rem;
  }

  p {
    font-size: 0.9rem;
  }
}

@media (max-width: 480px) {

  .overlay {
    display: flex;
    justify-content: center;
    flex-direction: column;
    height: 1vh;
  }

  h1 {
    width: 70vh;
    font-size: 1.5rem;
  }

  p {
    font-size: 0.9rem;
  }
}
</style>