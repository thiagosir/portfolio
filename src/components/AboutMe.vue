<script lang="ts">

export default {

}

</script>

<template>
  <div class="body">
    <div class="about">
      <h1 class="title">Sobre mim</h1>
      <p>
        Olá! Sou um entusiasta da tecnologia com um bacharelado em Sistemas de Informação, experiência em QA Automation
        e estou desenvolvendo meus conhecimentos em Vue e Laravel. Estou sempre buscando aprender novas linguagens e
        tecnologias, acreditando que isso me mantém atualizado e pronto para enfrentar desafios no setor de tecnologia.
        Estou aberto a novas oportunidades e desafios que possam me permitir aplicar e expandir minhas habilidades.
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
      <button class="button">
        <svg xmlns="http://www.w3.org/2000/svg" fill="white" viewBox="0 0 30 30" width="30px" height="30px">
          <path
            d="M15,3C8.373,3,3,8.373,3,15c0,5.623,3.872,10.328,9.092,11.63C12.036,26.468,12,26.28,12,26.047v-2.051 c-0.487,0-1.303,0-1.508,0c-0.821,0-1.551-0.353-1.905-1.009c-0.393-0.729-0.461-1.844-1.435-2.526 c-0.289-0.227-0.069-0.486,0.264-0.451c0.615,0.174,1.125,0.596,1.605,1.222c0.478,0.627,0.703,0.769,1.596,0.769 c0.433,0,1.081-0.025,1.691-0.121c0.328-0.833,0.895-1.6,1.588-1.962c-3.996-0.411-5.903-2.399-5.903-5.098 c0-1.162,0.495-2.286,1.336-3.233C9.053,10.647,8.706,8.73,9.435,8c1.798,0,2.885,1.166,3.146,1.481C13.477,9.174,14.461,9,15.495,9 c1.036,0,2.024,0.174,2.922,0.483C18.675,9.17,19.763,8,21.565,8c0.732,0.731,0.381,2.656,0.102,3.594 c0.836,0.945,1.328,2.066,1.328,3.226c0,2.697-1.904,4.684-5.894,5.097C18.199,20.49,19,22.1,19,23.313v2.734 c0,0.104-0.023,0.179-0.035,0.268C23.641,24.676,27,20.236,27,15C27,8.373,21.627,3,15,3z" />
        </svg>
      </button>
      <button class="button"></button>
      <button class="button"></button>
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
  margin-left: 500px;
}

.about {
  width: 500px;
}

.information {
  width: 300px;
}

.button:hover {
  color: #FF8000;
}

.button:hover .air {
  fill: #FF8000;
}
</style>