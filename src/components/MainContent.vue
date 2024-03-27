<script lang="ts">
import Header from '@/components/Header.vue'
import AboutMe from '@/components/AboutMe.vue'
import Footer from '@/components/Footer.vue'
import Knowledges from '@/components/Knowledges.vue'
import NavBar from '@/components/NavBar.vue'
import Experience from '@/components/Experience.vue'

export default {
  components: { Header, AboutMe, Footer, Knowledges, NavBar, Experience }
}
</script>

<template>
  <Header />
  <NavBar />
  <AboutMe />
  <Knowledges />
  <Experience />
  <Footer />
</template>