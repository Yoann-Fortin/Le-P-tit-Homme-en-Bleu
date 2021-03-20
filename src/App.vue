<template>
  <Header />
  <Home />
  <Footer />
</template>

<script>
import Header from './components/Header';
import Home from './components/Home';
import Footer from './components/Footer';


export default {
  name: 'App',
  components: {
    Header,
    Home,
    Footer
  }
}
</script>

<style>
  #app {
    max-width: 100vw;
    background-color: #d9e0f3;
    font-family: 'Yusei Magic', sans-serif;
    background-image: url('./assets/Background.svg');
    background-attachment: fixed;
    background-clip: content-box;
    background-repeat: no-repeat;
    background-size: 60rem;
    background-position: center bottom;
  }
</style>
