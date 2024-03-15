<script lang="ts">

export default {

}

</script>

<template>
  <div class="header">
    <div class="description">
      <p class="description_words">
        Olá! <br> Me chamo <span class="my_name">Thiago Couto</span> <br> e sou desenvolvedor full stack
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
  font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
  font-weight: 400;
  font-size: 33px;
}
.my_name {
  color: greenyellow;
}
.my_photo {
border-radius: 200px;
border: solid 3px;
border-color: greenyellow;
width: 300px;
height: 300px;

}
.image {
  margin-top: 150px;
  margin-right: 450px;
}
.description {
  margin-top: 150px;
  margin-left: 450px;;
}
</style>