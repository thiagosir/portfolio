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
  height: auto;
  justify-content: center;
  display: flex;
  flex-direction: column;
  color: white;
  font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
  gap: 1.25rem;
  padding: 1rem 0 1rem 0;
  margin-top: 6.25rem;
}

.body {
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
  width: 50%;
  height: 12.625rem;
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
  align-items: center;
  justify-content: space-between;
}

.nav-left-bar {
  height: 6.875rem;
  width: 100%;
  font-size: 1rem;
  border-style: solid;
  border-width: .0313rem;
  border-bottom: 0;
  border-right: 0;
  border-top: 0;
  border-color: #2f66c4;
}

.uninassau-text,
.cursos-text {
  padding-left: .625rem;
}

.uninassau {
  display: flex;
  align-items: center;
  height: 3.125rem;
  cursor: pointer;
  margin-bottom: .625rem;
  color: #a6adba;
}

.cursos {
  display: flex;
  align-items: center;
  height: 3.125rem;
  cursor: pointer;
  color: #a6adba
}

.cursos-style,
.uninassau-style {
  width: 90%;
}

.uninassau.active,
.cursos.active {
  border-color: #2f66c4;
  color: #2f66c4;
  transition: 0.1s;
  border-style: solid;
  border-bottom: 0;
  border-right: 0;
  border-top: 0;
}

@media screen and (max-width: 768px) {
  .container {
    display: flex;
    flex-direction: column;
  }
  
  .body {
    display: flex;
    flex-direction: column;
  }

  .div-left {
    display: flex;
    flex-direction: column;
    justify-content: start;
    width: 80%;
    background-color: #0f0e0e;
  }

  .text-experience {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 90%;
    height: 15.625rem;
  }
}
</style>
