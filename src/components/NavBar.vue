<script>

export default {

}
window.onscroll = function () { scrollFunction() };

function scrollFunction() {
  if (document.body.scrollTop > 20 || document.documentElement.scrollTop > 20) {
    document.getElementById("nav").style.top = "0";
  } else {
    document.getElementById("nav").style.top = "-50px";
  }
}
</script>

<template>
  <header class="header_nav">
    <ul class="nav">
      <li><a href="" class="nav_text">Sobre</a></li>
      <li><a href="" class="nav_text">Conhecimentos</a></li>
      <li><a href="" class="nav_text">Educação</a></li>
      <li><a href="" class="nav_text">Projetos</a></li>
      <li><a href="" class="nav_text">Experiência</a></li>
    </ul>
  </header>
</template>
<style scoped>
.header_nav {
  font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
  background-color: #14674f;
  align-items: center;
  justify-content: center;
  display: flex;
  height: 50px;
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
  transition: top 0.3s;
  position: fixed;
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