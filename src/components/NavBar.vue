<script>
export default {
  data() {
    return {
      isMenuOpen: false
    };
  },
  methods: {
    toggleMenu() {
      this.isMenuOpen = !this.isMenuOpen;
    }
  }
};
</script>

<template>
  <header class="header_nav" id="header_nav">
    <div class="scope">
      <img src="/src/assets/images/Icons/logo.svg" alt="Logo do site" class="img">
    </div>
    <div class="menu-style" @click="toggleMenu">
      <svg class="menu" v-if="!isMenuOpen" width="40px" height="40px" viewBox="0 0 24 24" fill="white"
        xmlns="http://www.w3.org/2000/svg">
        <path d="M4 6H20M4 12H20M4 18H20" stroke="#ffffff" stroke-width="2" stroke-linecap="round"
          stroke-linejoin="round" />
      </svg>
      <svg class="close" v-else width="40px" height="40px" viewBox="0 0 24 24" fill="white"
        xmlns="http://www.w3.org/2000/svg">
        <path d="M18 6L6 18M6 6L18 18" stroke="#ffffff" stroke-width="2" stroke-linecap="round"
          stroke-linejoin="round" />
      </svg>
    </div>
    <ul class="nav" :class="{ 'active': isMenuOpen }">
      <li><a href="#aboutme" class="nav_text">Sobre</a></li>
      <li><a href="#knowledge" class="nav_text">Conhecimentos</a></li>
      <li><a href="#experience" class="nav_text">Experiência</a></li>
      <li><a href="#projects" class="nav_text">Projetos</a></li>
      <li><a href="#education" class="nav_text">Educação</a></li>
    </ul>
  </header>
</template>

<style scoped>
.header_nav {
  font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
  background-color: #232D3F;
  align-items: center;
  justify-content: center;
  display: flex;
  height: 3.125rem;
  top: 0;
  position: fixed;
  width: 100%;
  transition: top 0.3s;
  z-index: 1;
}

.nav_text {
  display: block;
  padding: .5rem;
  text-decoration: none;
  color: white;
}

.nav {
  padding: 0;
  margin: 0;
  list-style-type: none;
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 1.876rem;
  width: 100%;
  transition: 0.5s;
}

.img {
  padding: 1rem;
}

.menu-style {
  display: none;
}

.menu-style svg {
  cursor: pointer;
}

.menu-style .close {
  display: none;
}

@media screen and (max-width: 768px) {
  .header_nav {
  justify-content: space-between;
  display: flex;

}
  .menu-style {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding-right: 1rem;
  }

  .nav {
    display: none;
    flex-direction: column;
    background-color: #232D3F;
    position: absolute;
    top: 3.125rem;
    left: 0;
    right: 0;
    padding: 1rem;
    z-index: 1;
  }

  .nav.active {
    display: flex;
  }

  .menu-style .menu {
    display: block;
  }

  .menu-style .close {
    display: block;
  }
}
</style>
