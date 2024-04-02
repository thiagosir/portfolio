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
          <div class="compass" @click="showExperience('compass')" :class="{'active': experienceSelected === 'compass'}"><span class="compass-text">Compass</span></div>
          <div class="gla" @click="showExperience('gla')" :class="{'active': experienceSelected === 'gla'}"><span class="gla-text">Jogador de GLA profissional</span></div>
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
          <a href="https://grandlineadventures.com/pt/" target="_blank" class="company">Grand Line Adventures</a>
          <p class="detail-experience">dou aula de como jogar gla da melhor maneira possível. Possuo uma gameplay de alto nível </p>
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
  gap: 50px;
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
  height: 112px;
  font-size: 16px;
  background-color: #0F0F0F;
}

.compass-text, .gla-text{
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

.gla {
  display: flex;
  align-items: center;
  height: 50px;
  cursor: pointer;
  color: #a6adba
}

.gla-style, .compass-style {
  width: 750px;
}

.compass.active, .gla.active {
  border-color: #2f66c4;
  color: #2f66c4;
  /* color: #4d6694; */
  transition: 0.1s;  
  border-style: solid;
  border-bottom: 0;
  border-right: 0;
  border-top: 0;
}

</style>
