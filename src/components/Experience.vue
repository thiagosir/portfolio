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
  height: 400px;
  justify-content: center;
  display: flex;
  flex-direction: column;
  color: white;
  font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
  gap: 20px;
}

.body {
  justify-content: center;
  align-items: center;
  display: flex;
  color: white;
  gap: 100px;
}

.div-left {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  width: 200px;
}

.company {
  text-decoration: none;
  color: white;
}

.company:hover {
  color: #4d6694;
}

.header {
  font-size: 38px;
  height: 100px;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
}

.text-experience {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 750px;
  height: 250px;
}

.title {
  display: flex;
  width: 750px;
  align-items: center;
  justify-content: space-between;
  margin-bottom: 20px;
}

.nav-left-bar {
  height: 110px;
  font-size: 16px;
  border-style: solid;
  border-width: 0.5px;
  border-bottom: 0;
  border-right: 0;
  border-top: 0;
  border-color: #2f66c4;
}

.compass-text,
.freelance-text {
  padding-left: 10px;
  width: 250px;
}

.compass {
  display: flex;
  align-items: center;
  height: 50px;
  cursor: pointer;
  margin-bottom: 10px;
  color: #a6adba;
}

.freelance {
  display: flex;
  align-items: center;
  height: 50px;
  cursor: pointer;
  color: #a6adba
}

.freelance-style,
.compass-style {
  width: 750px;
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
