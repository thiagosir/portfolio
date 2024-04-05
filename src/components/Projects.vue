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
          <a href="https://github.com/thiagosir/cookin-up" class="repository">Visualizar projeto</a>
        </article>
        <article class="projects">
          <h3 class="title">TrackerApp</h3>
          <p class="descrip">Projeto que permite a organização de seus projetos e tarefas do dia a dia. Também feito em Vuejs</p>
          <a href="https://github.com/thiagosir/tracker_vue" class="repository">Visualizar projeto</a>
        </article>
        <article class="projects">
          <h3 class="title">Automação de testes</h3>
          <p class="descrip">Projeto feito em Cypress para automatizar os testes da api ServeRest.</p>
          <a href="https://github.com/thiagosir/Automacao_Cypress_API_ServeRest" class="repository">Visualizar projeto</a>
        </article>
        <article class="projects">
          <h3 class="title">Node Lib</h3>
          <p class="descrip">Biblioteca em node que permite verificar quais textos e retornar links (se existirem no texto). Projeto feito em node.</p>
          <a href="https://github.com/thiagosir/node-lib-md" class="repository">Visualizar projeto</a>
        </article>
        <article class="projects">
          <h3 class="title">Em desenvolvimento...</h3>
          <p class="descrip">Aguarde um pouco enquanto desenvolvo mais algum projetinho felas...</p>
          <a href="github.com/thiagosir" class="repository">Visualizar projeto</a>
        </article>
        <article class="projects">
          <h3 class="title">Em desenvolvimento...</h3>
          <p class="descrip">Aguarde um pouco enquanto desenvolvo mais algum projetinho felas...</p>
          <a href="github.com/thiagosir" target="_blank" class="repository">Visualizar projeto</a>
        </article>
      </div>
    </div>
  </section>
</template>

<style scoped>
.container {
  width: 100%;
  height: 600px;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  display: flex;
  color: white;
  gap: 20px;
  font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
}

.body_projects {
  display: flex;
  justify-content: center;
  flex-direction: row;
  flex-wrap: wrap;
  width: 70%;
  height: 400px;
  gap: 20px;
}

.projects {
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 350px;
  height: 190px;
  border-style: solid;
  border-width: 1px;
  border-color: #4d6694;
  border-radius: 5px;
}

.projects:hover {
  transition: 1s;
  box-shadow: 8px 7px 10px #4d6694;
}

.descrip {
  width: 290px;
  height: 64px;
  font-size: 15px;
  color: #6e737d;
}

.title-project {
  font-size: 38px;
}

.repository {
  position: relative;
  text-decoration: none;
  color: #2f66c4;
}

.repository::before {
  content: '';
  position: absolute;
  bottom: -2px;
  left: 0;
  width: 0;
  height: 1px;
  background: linear-gradient(to right, #000000, #5b8dea);
  transition: width 0.3s ease;
}

.repository:hover::before {
  width: 100%;
}


</style>