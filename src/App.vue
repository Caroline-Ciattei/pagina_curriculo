<template>
<div class="home">
    <h2 class="home-titulo">Me chamo Caroline Ciatte,<strong class="home-titulo-destaque"> sou desenvolvedora Front-end.</strong></h2>
</div> 
<div class="card-container">
<div class="card mb-3 rounded" style="max-width: 35rem;">
  <div class="row g-0">
    <div class="col-md-4">
      <img src="./assets/foto.png" class="img-card" alt="Foto de perfil">
    </div>
    <div class="col-md-8">
      <div class="card-body mb-3 rounded">
        <h5 class="card-title">Sobre mim</h5><br>
        <p class="card-text">Sou apaixonada por tecnologia, adoro desenvolver páginas, usar a criatividade para estilizar o layout.</p>
        <p class="card-text">O mais legal para mim no mundo da Programação é estar sempre aprendendo coisas novas, sair do conforto dos conteúdos de conhecimento, pois nunca vamos saber tudo e sim ter motivação para sempre aprender coisas diferentes.</p>
      </div>
    </div>
  </div>
</div>
</div>
 <div class="fundo-card">
  <h2 class="titulo-card">Conhecimentos</h2>
  <card/>
<info/>
</div> 
  <footer class="rodape">
    <p class="texto-rodape">Desenvolvedora Caroline Ciattei</p>
  </footer>

</template>

<script>

import info from '@/components/info.vue';
import card from '@/components/card.vue';


export default {

  name: 'App',
  components: {
    card,
    info
  }
}

</script>

<style>

template {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
}

.home {
  display: flex;
  text-align: center;
  flex-direction: row;
  position: relative;
  width: 100%;
  margin: 0;
  color: #000000;
  align-items: center;
  height: 80vh; 
  overflow: hidden; 
  background-image: url('./assets/img-fundo.jpg');
  background-size: cover;
  background-position: center;
}

.home-titulo {
  font-size: 30px;
  font-weight: 700;
  display: flex;
  justify-content: center; 
  align-items: center; 
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  padding: 0;
  margin: 0; 
  white-space: nowrap;
  padding-left: 480px;
  padding-bottom: 260px;
} 

.home-titulo-destaque {
  color: rgb(169, 6, 117);
}

.card-body {
  background-color: #fcab86;
  height: 100%;
}

.card-title {
  font-weight: 800;
  font-size: 20px;
}

.card-text {
  font-weight: 700;
  font-size: 20px;
}

.img-card {
  width: 100%;
  height: auto;
}

.card-container {
  display: flex;
  justify-content: center; 
  align-items: center; 
  width: 100%;
  height: 100%;
  padding: 10px;
  background-color: #557494;
  padding-right: 30%;
}

.fundo-card {
  background-image: url(./assets/fundo-card.jpg);
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center; 
  height: 140vh;
}

.titulo-card {
  color: #000000;
  font-weight: 800;
  padding: 30px;
  padding-top: 100px;
  padding-left: 200px;
}

.g-0 {
  width: 150%;
  height: 100%;
}

.apresentacao {
  background-image: url('./assets/fundo-info.jpg');
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center; 
}

.rodape {
  background-color:  #5e93a0;
  color: #ffffff;
  position: absolute;
  bottom: 0;
  width: 100%;
  height: 10rem; 
  font-weight: bold; 
  font-size: 15px;
  text-shadow: 3px 2px 2px #e888d6;
  text-align: center;
  padding: 10px;
  position: fixed;
  height: auto;
}

.texto-rodape {
  padding-top: 10px;
}


@media screen and (max-width: 2560px) {

  .home {
    display: flex;
    flex-direction: column; 
    align-items: center;
    position: relative;
    width: 100%;
    justify-content: center;
    height: 100vh;
  }

  .home-titulo {
    font-weight: bold;
    margin-top: 40px;
    padding-right: 470px; 
    font-size: 30px;
  }

  .card {
   font-size: 50px;
  }

  .card-container {
    padding-right: 440px;
    font-size: 80%;
    height: 70vh;
    padding-left: 200px;
  }

  .titulo-card {
    padding-left: 760px;
    padding-bottom: 70px;
    font-size: 40px;
  }
  
  .fundo-card {
    width: 100%;
  }

  .card-text- {
    height: 90px;
    font-size: 15px;
  }

  .card-title {
    font-size: 35px;
  }

  .card-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(25rem, 1fr)); /* Altere o valor de 12rem para o tamanho desejado */
    gap: 20px;
    justify-items: center;
    align-items: center;
    padding: 20px;
    padding-left: 420px;
    padding-bottom: 200px;
    height: 100vh;
  }

  .titulo-card {
    padding-left: 1060px;
  }

  .apresentacao {
    padding-right: 220px;
    padding-top: 100px;
  }
  
  .apresentacao__links {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    gap: 60px;
    padding-top: 50px;
    padding-left: 110px;
}

  .apresentacao__links__navegacao {
    height: 70px;
    width: 260px;
    font-size: 23px;
  }

  .apresentacao__links__navegacao:focus {
    box-shadow: 0 0 5px rgba(0, 0, 0, 0.3);
  }

  .apresentacao__links__navegacao:hover {
    background-color: rgb(151, 240, 248);
    color: #b58ffc;
}

  .apresentacao__links__subtitulo {
    font-size: 35px;
    padding-top: 30px;
    padding-left: 120px;
  }

  .rodape {
    padding-right: 20px;
    font-size: 26px;
  }
}

</style>
