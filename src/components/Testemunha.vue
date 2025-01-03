<template>
  <div class="testimonial-container">
    <div class="avatar-section">
      <img src="../assets//imagens/feedback.png" alt="Avatar 1" class="avatar" />
    </div>
    <div class="quote-section">
      <h1 class="titulo-depoimento">
        Depoimentos:
      </h1>
      <p class="quote-text">
        "Lorem ipsum dolor sit amet consectetur adipisicing elit. Tenetur vitae pariatur aperiam, odit quod voluptates cumque voluptatem? Sunt dolorem, ducimus quasi neque libero"
      </p>
      <p class="author">Gabriel Lemos</p>
      <p class="location">São Paulo, SP</p>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'TestimonialComponent',
});
</script>

<style scoped>

.testimonial-container {
  justify-content: center;
  display: flex;
  align-items: center;
  text-align: left;
  font-size: 3vh;
  background-color: #34382E;
  height: 40rem;
  color: #fff;
  font-family: 'Arial', sans-serif;
}

.avatar-section {
  display: flex;
  flex-direction: column;
}

.avatar {
  width: 90%;
  height: 90%;
  object-fit: cover;
}

.quote-section {
  max-width: 600px;
}

.titulo-depoimento{
  font-size: 4vh;
}

.quote-text {
  font-size: 2vh;
  line-height: 1.5;
}

.author {
  font-size: 2vh;
  font-weight: bold;
  color: #fff;
}

.location {
  font-size: 15px;
  color: #fff;
}
</style>
