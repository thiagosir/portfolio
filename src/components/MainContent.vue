<script lang="ts">
import Header from '@/components/Header.vue'
import AboutMe from '@/components/AboutMe.vue'
import Footer from '@/components/Footer.vue'
import Knowledges from '@/components/Knowledges.vue'

export default {
  components: { Header, AboutMe, Footer, Knowledges }
}
</script>

<template>
  <Header />
  <AboutMe />
  <Knowledges />
  <Footer />
</template>