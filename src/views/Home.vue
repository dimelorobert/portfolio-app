<template>
  <div class="home">
    <Banner></Banner>
    <AboutMe></AboutMe>
    <Services></Services>
    <Projects></Projects>
    <Contact></Contact>
    <Footer></Footer>
  </div>
</template>

<script>
import Banner from '@/components/Banner.vue'
import AboutMe from '@/components/AboutMe.vue'
import Services from '@/components/Services.vue'
import Projects from '@/components/Projects.vue'
import Contact from '@/components/Contact.vue'
import Footer from '@/components/Footer.vue'

export default {
  name: 'Home',
  components: {
    Banner,
    AboutMe,
    Services,
    Projects,
    Contact,
    Footer
  }
}
</script>
