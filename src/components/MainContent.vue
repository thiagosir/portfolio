<script lang="ts">
import Header from '@/components/Header.vue'
import AboutMe from '@/components/AboutMe.vue'
import Footer from '@/components/Footer.vue'
import Knowledges from '@/components/Knowledges.vue'
import NavBar from '@/components/NavBar.vue'
import Experience from '@/components/Experience.vue'
import Projects from '@/components/Projects.vue'
import Education from '@/components/Education.vue'
import Curriculum from '@/components/Curriculum.vue'

export default {
  components: { Header, AboutMe, Footer, Knowledges, NavBar, Experience, Projects, Education, Curriculum }
}
</script>

<template>
  <Header />
  <NavBar />
  <AboutMe />
  <Knowledges />
  <Experience />
  <Projects />
  <Education />
  <Curriculum />
  <Footer />
</template>