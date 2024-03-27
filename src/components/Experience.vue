<script>
export default {
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
          <div class="compass" @click="showExperience('compass')">Compass</div>
          <div class="gla" @click="showExperience('gla')">Jogador profissional de GLA</div>
        </div>
      </div>
      <div class="text-experience">
        <div v-if="experienceSelected === 'compass'">
          <div class="title">
            <h4 class="title-experience">Desenvolvedor de automação de testes</h4>
            <p class="date">Mar 2022 - Set 2022 (6 meses)</p>
          </div>
          <h5 class="company">Compass.UOL</h5>
          <p class="detail-experience">Desenvolvi e automatizei testes utilizando o framework Cypress</p>
        </div>
        <div v-else-if="experienceSelected === 'gla'">
          <div class="title">
            <h4 class="title-experience">Experiência GLA</h4>
            <p class="date">Data GLA</p>
          </div>
          <h5 class="company">Empresa GLA</h5>
          <p class="detail-experience">Detalhes GLA</p>
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
}

.div-left {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  margin-right: 100px;
}

.header {
  font-size: 42px;
  padding-left: 800px;
  height: 100px;
}

.text-experience {
  justify-content: center;
  align-items: center;
  margin-left: 100px;
}

.date {
  margin-left: 50px;
}

.title {
  display: flex;
  align-items: center;
  margin-bottom: 50px;
}

.nav-left-bar {
  font-size: 16px;
}

.compass {
  cursor: pointer;
  border-style: solid;
  border-bottom: 0;
  border-right: 0;
  border-top: 0;
  border-color: #4d6694;
  margin-bottom: 10px;
}

.gla {
  cursor: pointer;
  border-style: solid;
  border-bottom: 0;
  border-right: 0;
  border-top: 0;
  border-color: #4d6694;
}
</style>
