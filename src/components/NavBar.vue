<script>
export default {

};
</script>

<template>
  <header class="header_nav" id="header_nav">
    <div class="scope">
      <img src="/src/assets/images/Icons/logo.svg" alt="Logo do site" class="img">
    </div>
    <div class="menu-style">
      <svg class="menu" width="40px" height="40px" viewBox="0 0 24 24" fill="white" xmlns="http://www.w3.org/2000/svg">
        <path d="M4 6H20M4 12H20M4 18H20" stroke="#161717" stroke-width="2" stroke-linecap="round"
          stroke-linejoin="round" />
      </svg>
    </div>
    <ul class="nav">
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
}

.img {
  padding: 1rem;
}

.nav_text:hover {
  transition: 0.5s;
  color: rgb(199, 197, 197);
}

.menu {
  display: none
}

@media screen and (max-width: 768px) {
  .nav {
    display: none;
  }

  .header_nav {
    justify-content: space-between;
  }

  .img {
    /* margin: .5rem; */
  }

  .menu {
    display: block;
    text-decoration: none;
    list-style-type: none;
    color: white;
    margin-right: 1.5rem;
    width: 100%;
    cursor: pointer;
  }

}
</style>