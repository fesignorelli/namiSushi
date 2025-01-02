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
    margin-top: 10vh;
    background-image: url('../assets/imagens/restauranteFundo.png'); /* Substitua pelo caminho da imagem */
    border-radius: 40px;
    background-size: 100% 100%;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
  }
  

  .overlay {
    background-color: rgba(88, 109, 75, 0.7); /* Fundo escuro com transparência */
    color: white;
    padding: 200px;
    border-radius: 40px;
    width: 100%;
    max-width: 800px;
  }
  
  h1 {
    font-size: 1.8rem;
    margin-bottom: 15px;
    font-weight: bold;
  }
  
  p {
    font-size: 1rem;
    line-height: 1.6;
  }

  @media (max-width: 768px) {
  h1 {
    font-size: 1.5rem;
  }

  p {
    font-size: 0.9rem;
  }
}

  </style>
  