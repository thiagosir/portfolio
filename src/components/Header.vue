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
          this.stars[i].top -= 1;
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
  color: #3f6c98;
  /* color: #14674f; */
}

.my_photo {
  border-radius: 200px;
  border: solid 2px;
  border-color: #232D3F;
  width: 300px;
  height: 300px;
}

.image {
  margin-top: 150px;
  margin-right: 500px;
  animation: slidein 1s ease-out, fadein 2s ease-out, slideinRight 1s ease-out;
}

.description {
  margin-top: 150px;
  margin-left: 500px;
  animation: slidein 1s ease-out, fadein 2s ease-out, slidein 1s ease-out;
}

.container {
  width: 100%;
  height: 700px;
  background: linear-gradient(0, #0F0F0F, #232D3F);
  /* background: linear-gradient(0, #000000, #006040); */
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

@keyframes slidein {
  from {
    opacity: 0;
    transform: translateX(-50px);
  }

  to {
    opacity: 1;
    transform: translateX(0);
  }
}

@keyframes slideinBelow {
  from {
    opacity: 0;
    transform: translateY(50px);
  }

  to {
    opacity: 1;
    transform: translateY(0);
  }
}

@keyframes slideinRight {
  from {
    opacity: 0;
    transform: translateX(50px);
  }

  to {
    opacity: 1;
    transform: translateX(0);
  }
}

@keyframes fadein {
  from {
    opacity: 0;
  }

  to {
    opacity: 1;
  }
}
</style>
