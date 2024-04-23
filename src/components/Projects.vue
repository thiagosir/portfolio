<script>
export default {

};
</script>

<template>
  <section id="projects" >
    <div class="container">
      <h2 class="title-project">Projetos</h2>
      <div class="body_projects">
        <article class="projects">
          <h3 class="title">CookinUp!</h3>
          <p class="descrip">Projeto com intuito de aprenziado, onde uso vários métodos que o Vuejs disponibiliza.</p>
          <a href="https://github.com/thiagosir/cookin-up" target="_blank" class="repository">Visualizar projeto</a>
        </article>
        <article class="projects">
          <h3 class="title">TrackerApp</h3>
          <p class="descrip">Projeto que permite a organização de seus projetos e tarefas do dia a dia. Também feito em Vuejs</p>
          <a href="https://github.com/thiagosir/tracker_vue" target="_blank" class="repository">Visualizar projeto</a>
        </article>
        <article class="projects">
          <h3 class="title">Automação de testes</h3>
          <p class="descrip">Projeto feito em Cypress para automatizar os testes da api ServeRest.</p>
          <a href="https://github.com/thiagosir/Automacao_Cypress_API_ServeRest" target="_blank" class="repository">Visualizar projeto</a>
        </article>
        <article class="projects">
          <h3 class="title">Node Lib</h3>
          <p class="descrip">Biblioteca em node que permite verificar quais textos e retornar links (se existirem no texto). Projeto feito em node.</p>
          <a href="https://github.com/thiagosir/node-lib-md" target="_blank" class="repository">Visualizar projeto</a>
        </article>
        <article class="projects">
          <h3 class="title">Freeway</h3>
          <p class="descrip">Joguinho da vaquinha atravessando a rua.</p>
          <a href="https://github.com/thiagosir/cow_game_js" target="_blank" class="repository">Visualizar projeto</a>
        </article>
        <article class="projects">
          <h3 class="title">Dev SignIn</h3>
          <p class="descrip">Projeto realizado com o intuito de aprender a utilizar o Banco de dados MongoDB, e algumas bibliotecas do Nestjs.</p>
          <a href="https://github.com/thiagosir/devsignin" target="_blank" class="repository">Visualizar projeto</a>
        </article>
      </div>
    </div>
  </section>
</template>

<style scoped>
.container {
  width: 100%;
  height: auto;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  display: flex;
  color: white;
  gap: 1.25rem;
  font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
}

.body_projects {
  display: flex;
  justify-content: center;
  flex-direction: row;
  flex-wrap: wrap;
  /* width: 70%; */
  height: auto;
  gap: 1.25rem;
}

.projects {
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 21.875rem;
  height: 11.875rem;
  border-style: solid;
  border-width: .0625rem;
  border-color: #4d6694;
  border-radius: .3125rem;
}

.projects:hover {
  transition: 1s;
  box-shadow: .5rem .4375rem .625rem #4d6694;
}

.descrip {
  width: 18.125rem;
  height: 4rem;
  font-size: .9375rem;
  color: #6e737d;
}

.title-project {
  font-size: 2.375rem;
}

.repository {
  position: relative;
  text-decoration: none;
  color: #2f66c4;
}

.repository::before {
  content: '';
  position: absolute;
  bottom: -0.125rem;
  left: 0;
  width: 0;
  height: .0625rem;
  background: linear-gradient(to right, #000000, #5b8dea);
  transition: width 0.3s ease;
}

.repository:hover::before {
  width: 100%;
}


</style>