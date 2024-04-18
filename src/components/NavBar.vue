<script>
export default {
  // mounted() {
  //   let prevScrollpos = window.scrollY;
  //   window.onscroll = function () {
  //     if (window.scrollY < 600) {
  //       document.getElementById("header_nav").style.top = "0";
  //       document.getElementById("header_nav").style.fixed;
  //     } else {
  //       let currentScrollPos = window.scrollY;
  //       if (prevScrollpos > currentScrollPos) {
  //         document.getElementById("header_nav").style.top = "-50px";
  //       } else {
  //         document.getElementById("header_nav").style.top = "0";
  //       }
  //       prevScrollpos = currentScrollPos;
  //     }
  //   };
  // },
};
</script>

<template>
  <header class="header_nav" id="header_nav">
    <a href="" class="menu">Menu</a>
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
  gap: 1.875rem;
  width: 100%;
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

  .menu {
    /* justify-content: end; */
    display: flex;
    /* position: absolute; */
    cursor: pointer;
    text-decoration: none;
    list-style-type: none;
    color: white;
  }

}
</style>