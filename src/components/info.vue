<template>
    <div class="apresentacao">
      <h2 class="apresentacao__links__subtitulo">Acesse minhas redes:</h2>
      <div class="apresentacao__links">
        <a class="apresentacao__links__navegacao" href="https://www.linkedin.com/in/caroline-ciattei-32a848237/">
          <img class="icon-link" src="../assets/icon-linkedin.png" alt="LinkedIn">
          Linkedin
        </a>
        <a class="apresentacao__links__navegacao" href="https://github.com/caroline-ciattei">
          <img class="icon-link" src="../assets/icon-github.png" alt="GitHub">
          GitHub
        </a>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'info'
  }
  </script>
  
  <style>
  
.apresentacao {
    height: 60vh;
    padding-top: 90px;
    text-align: center;
    padding-left: 70px;
}

  .apresentacao__links {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    gap: 30px;
    padding-top: 20px;
} 

.apresentacao__links__navegacao {
  text-decoration: none;
  display: flex; /* Usar display flex */
  align-items: center; /* Alinhar verticalmente o conteúdo */
  margin-bottom: 20px;
  margin-top: 20px; 
  padding: 15px 30px;
  border: 2px solid #9366b4;
  border-radius: 10px;
  transition: all 0.3s;
  color: #f3d36a;
  font-family: Arial, sans-serif;
  font-size: 18px;
  height: 70px;
  font-weight: 600;
}

.apresentacao__links__navegacao:focus {
  box-shadow: 0 0 5px rgba(0, 0, 0, 0.3);
}

.apresentacao__links__navegacao:hover {
  background-color: #9366b4;
  color: #ffffff;
}

.apresentacao__links__subtitulo {
  font-size: 30px;
  font-weight: 700;
  padding-top: 60px;
  margin-bottom: 20px;
}

.icon-link {
  width: 60px;
  height: 53px;
  margin-right: 10px;
}

</style>
  