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

<template>
  <div class="container">
    <div v-for="(star, index) in stars" :key="index" class="star"
      :style="{ top: star.top + 'px', left: star.left + 'px' }"></div>
    <div class="header">
      <div class="description">
        <p class="description_words">
          Olá! <br> Chamo-me <span class="my_name">Thiago Couto</span> <br> e sou desenvolvedor full stack.
        </p>
      </div>
      <div class="image">
        <img src="@/assets/images/portfolioImage.jpeg" alt="" class="my_photo">
      </div>
    </div>
  </div>
</template>

<style scoped>
.header {
  align-items: center;
  justify-content: center;
  display: flex;
  margin-top: 12rem;
  gap: 10rem;
}

.description_words {
  color: white;
  font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
  font-weight: 400;
  font-size: 2.1rem;
}

.my_name {
  color: #3f6c98;
}

.my_photo {
  border-radius: 12.5rem;
  border: solid;
  border-width: .125rem;
  border-color:  white;
  width: 19.75rem;
  height: 19.75rem;
}

.image {
  animation: slidein 1s ease-out, fadein 2s ease-out, slideinRight 1s ease-out;
  z-index: 1;

}

.description {
  animation: slidein 1s ease-out, fadein 2s ease-out, slidein 1s ease-out;
  z-index: 1;
}

.container {
  width: 100%;
  height: 43.75rem;
  background: linear-gradient(0, #0F0F0F, #232D3F);
  overflow: hidden;
  position: relative;
}

.star {
  width: .1875rem;
  height: .1875rem;
  position: absolute;
  border-radius: 50%;
  background-color: white;
}

@keyframes slidein {
  from {
    opacity: 0;
    transform: translateX(-3.125rem);
  }
  
  to {
    opacity: 1;
    transform: translateX(0);
  }
}

@keyframes slideinBelow {
  from {
    opacity: 0;
    transform: translateY(3.125rem);
  }
  
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

@keyframes slideinRight {
  from {
    opacity: 0;
    transform: translateX(3.125rem);
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
@media screen and (max-width: 768px) {
  .container{
    width: 100%;
    margin-bottom: -10rem;
  }
  .image {
    margin-top: 5rem;
    animation: slidein 1s ease-out, fadein 2s ease-out, slideinRight 1s ease-out;
    z-index: 1;
  }
  
  .description {
    animation: slidein 1s ease-out, fadein 2s ease-out, slidein 1s ease-out;
    z-index: 1;
  }
  
  .header {
    display: flex;
    flex-direction: column-reverse;
    justify-content: center;
    margin-top: 5rem;
    gap: 1rem;
  }
  .description_words {
    font-size: 1.2rem;
  }
  .my_photo {
    width: 10.75rem;
    height: 10.75rem;
  }
}

@media screen and (min-width: 769px) and (max-width: 1024px) {
  .container{
    width: 100%;
  }
  .image {
    margin-top: 5rem;
    animation: slidein 1s ease-out, fadein 2s ease-out, slideinRight 1s ease-out;
    z-index: 1;
  }
  
  .description {
    animation: slidein 1s ease-out, fadein 2s ease-out, slidein 1s ease-out;
    z-index: 1;
  }
  
  .header {
    display: flex;
    flex-direction: column-reverse;
    justify-content: center;
    margin-top: 5rem;
    gap: 1.8rem;
  }
  .description_words {
    font-size: 2rem;
  }
  .my_photo {
    width: 18.75rem;
    height: 18.75rem;
  }
}

</style>
