<script lang="ts">

export default {

}

</script>

<template>
  <div class="header">
    <div class="description">
      <p class="description_words">
        Olá! Eu sou o <span class="my_name">Thiago Couto</span> e sou desenvolvedor full stack
      </p>
    </div>
    <div class="image">
      <img src="@/assets/myPic.jpeg" alt="" class="my_photo">
    </div>
  </div>
</template>

<style scoped>
.header {
  align-items: center;
  justify-content: space-between;

  display: flex;
  gap: 15px;
}
.description_words {
  color: white;
}
.my_name {
  color: greenyellow;
}
.my_photo {
border-radius: 200px;
width: 200px;
height: 200px;
}
.image {
  margin-right: 250px;
}
.description {
  margin-left: 250px;;
}
</style>