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
  <main class="container">
    <div class="header">Experiências</div>
    <div class="body">
      <div class="div-left">
        <div class="nav-left-bar">
          <div class="compass" @click="showExperience('compass')" :class="{'active': experienceSelected === 'compass'}">Compass</div>
          <div class="gla" @click="showExperience('gla')" :class="{'active': experienceSelected === 'gla'}">Jogador profissional de GLA</div>
        </div>
      </div>
      <div class="text-experience">
        <div class="compass-style" v-if="experienceSelected === 'compass'">
          <div class="title">
            <h4 class="title-experience">Desenvolvedor de automação de testes</h4>
            <p class="date">Mar 2022 - Set 2022 (6 meses)</p>
          </div>
          <a href="https://compass.uol/pt/home/" target="_blank" class="company">Compass.UOL</a>
          <p class="detail-experience">Desenvolvi e automatizei testes utilizando o framework Cypress</p>
        </div>
        <div class="gla-style" v-else-if="experienceSelected === 'gla'">
          <div class="title">
            <h4 class="title-experience">Grande jogador de gla</h4>
            <p class="date">Jan 2024 - Atual</p>
          </div>
          <h5 class="company">Grand Line Adventures</h5>
          <p class="detail-experience">dou aula de como jogar gla da melhor maneira possível. Possuo uma gameplay de alto nível</p>
        </div>
      </div>
    </div>
  </main>
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
}

.body {
  margin-top: 70px;
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
  margin-right: 100px;
}

.company {
  text-decoration: none;
  color: white;
}

.company:hover {
  color: #4d6694;
}

.header {
  font-size: 42px;
  padding-left: 800px;
  height: 100px;
}

.text-experience {
  justify-content: center;
  align-items: center;
  width: 700px
}

.date {
  margin-left: 50px;
}

.title {
  display: flex;
  align-items: center;
  margin-bottom: 20px;
}

.nav-left-bar {
  font-size: 16px;
}

.compass {
  display: flex;
  align-items: center;
  height: 30px;
  cursor: pointer;
  border-style: solid;
  border-bottom: 0;
  border-right: 0;
  border-top: 0;
  margin-bottom: 10px;
}

.gla {
  display: flex;
  align-items: center;
  height: 30px;
  cursor: pointer;
  border-style: solid;
  border-bottom: 0;
  border-right: 0;
  border-top: 0;
}

.gla-style {
  
}

.compass.active {
  background: #161717;
  border-color: #4d6694;
  color: white;
}

.gla.active {
  background: #161717;
  border-color: #4d6694;
  color: white;
}
</style>
