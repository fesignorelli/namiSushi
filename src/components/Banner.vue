<script lang="ts">
export default {
    name: "App",
};
</script>

<template>
    <main class="main-content">

        <div class="image-content">
            <img src="../assets//imagens/logoBanner.png" alt="Sushi" />
        </div>

        <div class="text-content">
            <h1>
                um bom <span class="highlight">sushi</span>, <br />
                um bom <span class="highlight">humor!</span>
            </h1>
            <p>Está com fome? Acabe com ela já! Veja agora seu cardápio:</p>
            <button class="menu-button">clique aqui:</button>
        </div>

    </main>
</template>



<style scoped>
.main-content {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 20vh;
    margin-top: 5%;
}

.text-content {
    font-family: 'Times New Roman', Times, serif;
    text-align: left;
}

.text-content h1 {
    color: #000;
    font-size: 3rem;
    line-height: 1.5;
}

.text-content .highlight {
    color: #173c1c;
    font-weight: bold;
}

.text-content p {
    color: #000;
    font-size: 1.6rem;
    width: 60%;
    font-weight: 500;
}

.menu-button {
    background-color: #173c1c;
    color: white;
    border: none;
    padding: 10px 20px;
    cursor: pointer;
    font-size: 1.4rem;
    border-radius: 5px;
}

.image-content img {
    max-width: 400px;
}

@media (max-width: 768px) {
    .main-content {
        flex-direction: column;
        align-items: center;
        gap: 20px;
    }

    .text-content {
        text-align: center;
        margin-bottom: 2vh;
    }

    .text-content h1 {
        font-size: 2rem;
    }

    .text-content p {
        font-size: 3vh;
        max-width: 70%;
    }

    .image-content img {
        max-width: 50%;
    }
}

@media (max-width: 480px) {

    .image-content {
        display: flex;
        justify-content: center;
        margin: 0;
        align-items: center;
    }

    .text-content {
        align-items: center;
        text-align: center;
    }

    .text-content h1 {
        font-size: 2rem;
    }

    .text-content p {
        display: flex;
        justify-content: center;
        align-items: center;
        margin: 0 auto;
        text-align: center;
        font-size: 1.3rem;
        width: 70%;
    }

    .menu-button {
        translate: 0 2vh;
        font-size: 1.5rem;
        padding: 8px 16px;
    }
}
</style>