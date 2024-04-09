<script lang="ts">

export default {

}

</script>

<template>
  <section id="aboutme">
    <main class="main">
      <div class="body">
        <div class="top-section">
          <div class="about">
            <h1 class="title">Sobre mim</h1>
            <p>
              Olá! Sou um entusiasta da tecnologia com um bacharelado em Sistemas de Informação, experiência em QA
              Automation
              e estou desenvolvendo meus conhecimentos em Vue e Laravel. Estou sempre buscando aprender novas linguagens
              e
              tecnologias, acreditando que isso me mantém atualizado e pronto para enfrentar desafios no setor de
              tecnologia.
              Estou aberto a novas oportunidades e desafios que possam me permitir aplicar e expandir minhas
              habilidades.
            </p>
          </div>
          <div class="information">
            <h1 class="title">Informações</h1>
            <div class="spans">
              <span class="dataTitle">Idade: </span><span class="dataRes">22 anos</span> <br>
              <span class="dataTitle">Email: </span> <span class="dataRes">bentothiago57@gmail.com</span><br>
              <span class="dataTitle">Telefone: </span> <span class="dataRes">+55 (88) 981686490</span><br>
              <span class="dataTitle">Localização: </span> <span class="dataRes">Araripina, Pernambuco,
                Brasil</span><br>
              <span class="dataTitle">Idiomas: </span> <span class="dataRes">Português, Inglês.</span><br>
            </div>
          </div>
        </div>
        <div class="socials">
          <a href="https://github.com/thiagosir" class="button" target="_blank">
            <svg width="30px" height="30px" viewBox="0 0 48 48" id="Layer_2" data-name="Layer 2" fill="white" class="svg"
              xmlns="http://www.w3.org/2000/svg">
              <path
                d="M24,2.5a21.5,21.5,0,0,0-6.8,41.9c1.08.2,1.47-.46,1.47-1s0-1.86,0-3.65c-6,1.3-7.24-2.88-7.24-2.88A5.7,5.7,0,0,0,9,33.68c-1.95-1.33.15-1.31.15-1.31a4.52,4.52,0,0,1,3.29,2.22c1.92,3.29,5,2.34,6.26,1.79a4.61,4.61,0,0,1,1.37-2.88c-4.78-.54-9.8-2.38-9.8-10.62a8.29,8.29,0,0,1,2.22-5.77,7.68,7.68,0,0,1,.21-5.69s1.8-.58,5.91,2.2a20.46,20.46,0,0,1,10.76,0c4.11-2.78,5.91-2.2,5.91-2.2a7.74,7.74,0,0,1,.21,5.69,8.28,8.28,0,0,1,2.21,5.77c0,8.26-5,10.07-9.81,10.61a5.12,5.12,0,0,1,1.46,4c0,2.87,0,5.19,0,5.9s.39,1.24,1.48,1A21.5,21.5,0,0,0,24,2.5" />
            </svg>
          </a>
          <a href="https://www.linkedin.com/in/thiago-couto-b95635243/" class="button" target="_blank">
            <svg width="30px" height="30px" viewBox="0 0 24 24" fill="white" xmlns="http://www.w3.org/2000/svg" class="svg">
            <path
              d="M6.5 8C7.32843 8 8 7.32843 8 6.5C8 5.67157 7.32843 5 6.5 5C5.67157 5 5 5.67157 5 6.5C5 7.32843 5.67157 8 6.5 8Z"
               />
            <path
              d="M5 10C5 9.44772 5.44772 9 6 9H7C7.55228 9 8 9.44771 8 10V18C8 18.5523 7.55228 19 7 19H6C5.44772 19 5 18.5523 5 18V10Z"
               />
            <path
              d="M11 19H12C12.5523 19 13 18.5523 13 18V13.5C13 12 16 11 16 13V18.0004C16 18.5527 16.4477 19 17 19H18C18.5523 19 19 18.5523 19 18V12C19 10 17.5 9 15.5 9C13.5 9 13 10.5 13 10.5V10C13 9.44771 12.5523 9 12 9H11C10.4477 9 10 9.44772 10 10V18C10 18.5523 10.4477 19 11 19Z"
               />
            <path fill-rule="evenodd" clip-rule="evenodd"
              d="M20 1C21.6569 1 23 2.34315 23 4V20C23 21.6569 21.6569 23 20 23H4C2.34315 23 1 21.6569 1 20V4C1 2.34315 2.34315 1 4 1H20ZM20 3C20.5523 3 21 3.44772 21 4V20C21 20.5523 20.5523 21 20 21H4C3.44772 21 3 20.5523 3 20V4C3 3.44772 3.44772 3 4 3H20Z"
               />
            </svg>
          </a>
        </div>
      </div>
    </main>
  </section>
</template>
<style scoped>
.main {
  display: flex;
  justify-content: center;
  margin-top: 150px;
}

.body {
  width: 65%;
  height: 350px;
  border-radius: 15px;
  background-color: #161717;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.top-section {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  gap: 40px;
}

.about {
  color: white;
  width: 500px;
  margin-right: 100px;
  font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
  animation: slidein 1s ease-out, fadein 2s ease-out;
}

.information {
  color: white;
  font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
  animation: slidein 1s ease-out, fadein 2s ease-out, slideinRight 1s ease-out;
  width: 300px;
}

.socials {
  margin-top: 30px;
  /* ease-out: Começa rápido e desacelera à medida que a animação progride */
  animation: slidein 1s ease-out, fadein 2s ease-out, slideinBelow 1s ease-out;
}

@keyframes slidein {
  from {
    opacity: 0;
    transform: translateX(-50px);
  }

  to {
    opacity: 1;
    transform: translateX(0);
  }
}

@keyframes slideinBelow {
  from {
    opacity: 0;
    transform: translateY(50px);
  }

  to {
    opacity: 1;
    transform: translateY(0);
  }
}

@keyframes slideinRight {
  from {
    opacity: 0;
    transform: translateX(50px);
  }

  to {
    opacity: 1;
    transform: translateX(0);
  }
}

@keyframes fadein {
  from {
    opacity: 0;
  }

  to {
    opacity: 1;
  }
}

.button:hover {
  color: #008170;
  border: none !important;
  cursor: pointer;
}

.button {
  margin: 5px;
}

.button:hover .svg {
  fill: #4d6694;
}

.dataTitle,
.dataRes {
  line-height: 25px;
  font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
}
</style>