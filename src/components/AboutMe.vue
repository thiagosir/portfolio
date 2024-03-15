<script lang="ts">

export default {
  
}

</script>

<template>
  <div class="body">
    <div class="about">
      <h1 class="title">Sobre mim</h1>
      <p>
        Olá! Sou um entusiasta da tecnologia com um bacharelado em Sistemas de Informação, experiência em QA Automation e estou desenvolvendo meus conhecimentos em Vue e Laravel. Estou sempre buscando aprender novas linguagens e tecnologias, acreditando que isso me mantém atualizado e pronto para enfrentar desafios no setor de tecnologia. Estou aberto a novas oportunidades e desafios que possam me permitir aplicar e expandir minhas habilidades.
      </p>
    </div>
    <div class="information">
      <h1 class="title">Informações</h1>
      <div class="spans">
        <span class="dataTitle">Idade: </span><span class="dataRes">23 anos</span> <br>
        <span class="dataTitle">Email: </span> <span class="dataRes">bentothiago57@gmail.com</span><br>
        <span class="dataTitle">Telefone: </span> <span class="dataRes">+55 (88) 981686490</span><br>
        <span class="dataTitle">Localização: </span> <span class="dataRes">Araripina, Pernambuco, Brasil</span><br>
        <span class="dataTitle">Idiomas: </span> <span class="dataRes">Português, Inglês.</span><br>
      </div>
    </div>
    <div class="socials">
      
    </div>
  </div>
</template>
<style scoped>
  .body {
    display: flex;
    align-items: center;
    justify-content: center;
    background-color: grey;
    border-radius: 15px;
    width: 900px;
    margin-left: 500px ;
  }
  .about {
    width: 500px;
  }
  .information {
    width: 300px;

  }
</style>