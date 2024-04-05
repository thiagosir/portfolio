<script>
export default {
  props: {
    active: Boolean
  },
  data() {
    return {
      experienceSelected: 'uninassau'
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
  <section id="education">
    <main class="container">
      <div class="header">Educação</div>
      <div class="body">
        <div class="div-left">
          <div class="nav-left-bar">
            <div class="uninassau" @click="showExperience('uninassau')" :class="{ 'active': experienceSelected === 'uninassau' }">
              <span class="uninassau-text">UNINASSAU</span></div>
            <div class="cursos" @click="showExperience('cursos')" :class="{ 'active': experienceSelected === 'cursos' }"><span
                class="cursos-text">Cursos em geral</span></div>
          </div>
        </div>
        <div class="text-experience">
          <div class="uninassau-style" v-if="experienceSelected === 'uninassau'">
            <div class="title">
              <h4 class="title-experience">Bacharelado em Sistemas de Informação</h4>
              <p class="date">Fev 2019 - Dez 2022 (4 anos)</p>
            </div>
            <p class="detail-experience">Centro Universitário Maurício de Nassau - UNINASSAU</p>
          </div>
          <div class="cursos-style" v-else-if="experienceSelected === 'cursos'">
            <div class="title">
              <h4 class="title-experience">Cursos</h4>
              <p class="date">Jan 2023 - Atual (1 ano e 4 meses)</p>
            </div>
            <p class="detail-experience">Vários cursos sobre programação nas plataformas da Alura, Udemy, DIO e RocketSeat</p>
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
  height: 350px;
  justify-content: center;
  display: flex;
  flex-direction: column;
  color: white;
  font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
  margin-top: 100px;
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
  height: 10px;
  margin-top: 50px;
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

.title-experience {
  font-size: large;
  font-weight: 500;
}

.detail-experience {
  color: #6e737d;
}

.title {
  display: flex;
  width: 750px;
  align-items: center;
  justify-content: space-between;
  margin-bottom: -30px;
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

.uninassau-text,
.cursos-text {
  padding-left: 10px;
  width: 250px;
}

.uninassau {
  display: flex;
  align-items: center;
  height: 50px;
  cursor: pointer;
  margin-bottom: 10px;
  color: #a6adba;
}

.cursos {
  display: flex;
  align-items: center;
  height: 50px;
  cursor: pointer;
  color: #a6adba
}

.cursos-style,
.uninassau-style {
  width: 750px;
}

.uninassau.active,
.cursos.active {
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
