<script lang="ts">
export default {
    name: "App",
};
</script>

<template>
    <main class="main-content">
        <div class="text-content">
            <h1>
                um bom <span class="highlight">sushi</span>, <br />
                um bom <span class="highlight">humor!</span>
            </h1>
            <p>Está com fome? Acabe com ela já! Veja agora seu cardápio:</p>
            <button class="menu-button">clique aqui:</button>
        </div>
        <div class="image-content">
            <img src="../assets//imagens/logoBanner.png" alt="Sushi" />
        </div>
    </main>
</template>



<style scoped>

.main-content {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-top: 5rem;
    flex-wrap: wrap;
}

.text-content {
    text-align: left;
    max-width: 50%;
}

.text-content h1 {
    color: #fff;
    font-size: 3rem;
    line-height: 1.5;
}

.text-content .highlight {
    color: #8b8b56;
    font-weight: bold;
}

.text-content p {
    color: #fff;
    font-size: 1.6rem;
    font-weight: 500;
}

.menu-button {
    background-color: #8b8b56;
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
        text-align: center;
    }

    .text-content {
        max-width: 100%;
        margin-bottom: 20px;
    }

    .image-content img {
        max-width: 80%;
        margin: 0 auto;
    }
}

@media (max-width: 480px) {
    .header nav ul {
        flex-direction: column;
        gap: 10px;
    }

    .header .icons {
        display: flex;
        justify-content: center;
        gap: 10px;
    }

    .text-content h1 {
        font-size: 1.5rem;
    }

    .text-content p {
        font-size: 1rem;
    }

    .menu-button {
        font-size: 0.9rem;
        padding: 8px 16px;
    }
}
</style>