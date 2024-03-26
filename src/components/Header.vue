<template>
  <div class="container">
    <div v-for="(star, index) in stars" :key="index" class="star"
      :style="{ top: star.top + 'px', left: star.left + 'px' }"></div>
    <div class="header">
      <div class="description">
        <p class="description_words">
          Olá! <br> Me chamo <span class="my_name">Thiago Couto</span> <br> e sou desenvolvedor full stack
        </p>
      </div>
      <div class="image">
        <img src="@/assets/images/myPic.jpeg" alt="" class="my_photo">
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      stars: []
    };
  },
  mounted() {
    this.createStars();
    this.animateStars();
  },
  methods: {
    createStars() {
      for (let i = 0; i < 100; i++) {
        this.stars.push({
          top: Math.random() * window.innerHeight,
          left: Math.random() * window.innerWidth
        });
      }
    },
    animateStars() {
      setInterval(() => {
        for (let i = 0; i < this.stars.length; i++) {
          this.stars[i].top -= 1; // Subtraindo um valor fixo para mover para cima suavemente
          if (this.stars[i].top < -10) this.stars[i].top = window.innerHeight;
        }
      }, 50);
    }
  }
};
</script>

<style scoped>
.header {
  /* padding-top: 150px; */
  align-items: center;
  justify-content: space-between;
  display: flex;
}

.description_words {
  color: white;
  font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
  font-weight: 400;
  font-size: 33px;
}

.my_name {
  color: #14674f;
}

.my_photo {
  border-radius: 200px;
  border: solid 3px;
  border-color: #14674f;
  width: 300px;
  height: 300px;
}

.image {
  margin-top: 150px;
  margin-right: 500px;
}

.description {
  margin-top: 150px;
  margin-left: 500px;
}

.container {
  width: 100%;
  height: 700px;
  background: linear-gradient(0, #006040, #000000);
  overflow: hidden;
  position: relative;
}

.star {
  width: 3px;
  height: 3px;
  position: absolute;
  border-radius: 50%;
  background-color: white;
}
</style>
