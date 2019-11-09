<template>
  <div id="home">
    <NavBar />
    <Home />
    <NewsLetter />
    <Boxes />
    <About />
    <Authors />
    <Contact />
    <Footer />
  </div>
</template>

<script>
import NavBar from '@/components/NavBar'
import Home from '@/components/Home'
import NewsLetter from '@/components/NewsLetter'
import Boxes from '@/components/Boxes'
import About from '@/components/About'
import Authors from '@/components/Authors'
import Contact from '@/components/Contact'
import Footer from '@/components/Footer'

export default {
  name: "app",
  components: {
    NavBar,
    Home,
    NewsLetter,
    Boxes,
    About,
    Authors,
    Contact,
    Footer
  }
};
</script>

<style>
/* #app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
} */
</style>
