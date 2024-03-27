<script>
export default {

};

</script>

<template>
  <main class="container">
    <div class="header">Experiências</div>
    <div class="body">
      <div class="div-left">
        <div class="nav-left-bar">
          <div class="compass">Compass</div>
          <div class="gla">Jogador de GLA</div>
        </div>
      </div>
      <div class="text-experience">
        <div class="title">
          <h4 class="title-experience">Desenvolvedor de automação de testes</h4>
          <p class="date">Mar 2022 - Set 2022 (6 meses)</p>
        </div>
        <h5 class="company">Compass.UOL</h5>
        <p class="detail-experience">Testa a dor</p>
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
  color: white;
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
}
.text-experience {
  justify-content: center;
  align-items: center;
}
.date {
 margin-left: 50px;
}
.title {
  display: flex;
  align-items: center;
  margin-bottom: 50px;
}
</style>