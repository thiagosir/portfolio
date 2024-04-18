<script>
export default {
  props: {
    active: Boolean
  },
  data() {
    return {
      experienceSelected: 'compass'
    }
  },
  methods: {
    showExperience(experience) {
      this.experienceSelected = experience;
    }
  }
};
</script>
<template>
  <section id="experience">
    <main class="container">
      <div class="header">Experiências</div>
      <div class="body">
        <div class="div-left">
          <div class="nav-left-bar">
            <div class="compass" @click="showExperience('compass')" :class="{ 'active': experienceSelected === 'compass' }">
              <span class="compass-text">Compass</span></div>
            <div class="freelance" @click="showExperience('freelance')" :class="{ 'active': experienceSelected === 'freelance' }"><span
                class="freelance-text">Freelancer</span></div>
          </div>
        </div>
        <div class="text-experience">
          <div class="compass-style" v-if="experienceSelected === 'compass'">
            <div class="title">
              <h4 class="title-experience">Desenvolvedor de automação de testes</h4>
              <p class="date">Mar 2022 - Set 2022 (6 meses)</p>
            </div>
            <a href="https://compass.uol/pt/home/" target="_blank" class="company">Compass.UOL</a>
            <p class="detail-experience">Atuei no desenvolvimento de automação de testes back-end e front-end utilizando a ferramenta Cypress. Também atuei no desenvolvimento de testes manuais na API utilizando o Postman.</p>
          </div>
          <div class="freelance-style" v-else-if="experienceSelected === 'freelance'">
            <div class="title">
              <h4 class="title-experience">Comanda digital para restaurantes</h4>
              <p class="date">Ago 2023 - Atual (8 meses)</p>
            </div>
            <p class="detail-experience">Atualmente participo como desenvolvedor back-end utilizando a linguagem Nestjs para o desenvolvimento de uma comanda digital projetada para modernizar e otimizar o processo de pedidos e pagamentos em restaurantes.</p>
          </div>
        </div>
      </div>
    </main>
  </section>
</template>


<style scoped>
.container {
  background-color: #161717;
  width: 100%;
  height: 25rem;
  justify-content: center;
  display: flex;
  flex-direction: column;
  color: white;
  font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
  gap: 1.25rem;
}

.body {
  justify-content: center;
  align-items: center;
  display: flex;
  color: white;
  gap: 6.25rem;
}

.div-left {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  /* width: 12.5rem; */
}

.company {
  text-decoration: none;
  color: white;
}

.company:hover {
  color: #4d6694;
}

.header {
  font-size: 2.375rem;
  height: 6.25rem;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
}

.text-experience {
  display: flex;
  justify-content: center;
  align-items: center;
  /* width: 46.875rem; */
  height: 15.625rem;
}

.title {
  display: flex;
  /* width: 46.875rem; */
  align-items: center;
  justify-content: space-between;
  margin-bottom: 1.25rem;
}

.nav-left-bar {
  height: 6.875rem;
  font-size: 1rem;
  border-style: solid;
  border-width: .0313rem;
  border-bottom: 0;
  border-right: 0;
  border-top: 0;
  border-color: #2f66c4;
}

.compass-text,
.freelance-text {
  padding-left: .625rem;
  /* width: 15.625rem; */
}

.compass {
  display: flex;
  align-items: center;
  height: 3.125rem;
  cursor: pointer;
  margin-bottom: .625rem;
  color: #a6adba;
}

.freelance {
  display: flex;
  align-items: center;
  height: 3.125rem;
  cursor: pointer;
  color: #a6adba
}

.freelance-style,
.compass-style {
  /* width: 46.875rem; */
}

.compass.active,
.freelance.active {
  border-color: #2f66c4;
  color: #2f66c4;
  transition: 0.1s;
  border-style: solid;
  border-bottom: 0;
  border-right: 0;
  border-top: 0;
}
</style>
