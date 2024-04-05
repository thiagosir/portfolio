<script>
export default {
  mounted() {
    let prevScrollpos = window.scrollY;
    window.onscroll = function () {
      let currentScrollPos = window.scrollY;
      if (prevScrollpos > currentScrollPos) {
        document.getElementById("header_nav").style.top = "-50px";
      } else {
        document.getElementById("header_nav").style.top = "0";
      }
      prevScrollpos = currentScrollPos;
    };
  },
};
</script>

<template>
  <header class="header_nav" id="header_nav">
    <ul class="nav">
      <li><a href="#aboutme" class="nav_text">Sobre</a></li>
      <li><a href="#knowledge" class="nav_text">Conhecimentos</a></li>
      <li><a href="#experience" class="nav_text">Experiência</a></li>
      <li><a href="#education" class="nav_text">Educação</a></li>
      <li><a href="#projects" class="nav_text">Projetos</a></li>
    </ul>
  </header>
</template>

<style scoped>
.header_nav {
  font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
  /* background-color: transparent; */
  background-color: #232D3F;
  /* background: linear-gradient(0, #006040, #000000); */
  align-items: center;
  justify-content: center;
  display: flex;
  height: 50px;
  top: 0;
  position: fixed;
  width: 100%;
  transition: top 0.3s;
}

.nav_text {
  display: block;
  padding: 8px;
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
  gap: 30px;
  width: 100%;
}

.nav a:hover {
  /* background-color: aqua; */
}
</style>