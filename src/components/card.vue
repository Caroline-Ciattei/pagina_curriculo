<template>
  <div class="card-grid">
    <div class="card-" v-for="(card, index) in cards" :key="index">
      <img :src="card.image" class="card-img-top" :alt="card.title">
      <div class="card--body-">
        <h5 class="card-title-">{{ card.title }}</h5>
        <p class="card-text-">{{ card.description }}</p>
      </div>
    </div>
  </div>
</template>


<script>
export default {
  data() {
    return {
      cards: [
        {
          title: 'Vue.js',
          description: 'É um framework progressivo para a construção de interfaces de usuário.',
          image: '/img/icon-vue.js.png',
        },
        {
          title: 'JavaScript',
          description: 'É uma linguagem de programação que permite a você implementar itens complexos em páginas web.',
          image: '/img/imagem-javascript.png',
        },
        {
          title: 'HTML',
          description: 'É uma linguagem de marcação utilizada para estruturar os elementos da página.',
          image: '/img/icon-html.png',
        },
        {
          title: 'CSS',
          description: 'É uma linguagem de estilização utilizada para definir cores, fontes, e qualquer outro valor estético para os elementos da página.',
          image: '/img/imagem-Css.png',
        },
      ],
    };
  },
};
</script>


<style>
/* Estilos personalizados */

.card-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(18rem, 1fr)); 
  gap: 20px; /* Espaço entre os cards */
  justify-items: center; /* Centralizar horizontalmente */
  align-items: center; 
  padding-left: 30%;
  padding-right: 40px;
}

.card- {
  width: 100%;
  height: 350px;
  box-shadow: 5px 5px 5px #743198;
  transition: transform 0.3s;
}

.card-:hover {
  transform: scale(1.05);
}

.card-img-top {
  width: 100%;
  height: 200px;
  object-fit: scale-down;
  background-color: #ffffff;
}

.card--body- {
  padding: 8px;
  background-color: #f3c790;
}

.card-title- {
  font-size: 1.25rem;
  font-weight: bold;
}

.card-text- {
  font-size: 1rem;
  color: #000000;
  height: 100px;
}

</style>




