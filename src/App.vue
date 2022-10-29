<template>
  <div id="app">
    <nav-menu :pages="pages"></nav-menu>
    <router-view class="wrapper"></router-view>
    <footer-bar></footer-bar>
  </div>
</template>

<script>
import NavMenu from './components/Nav.vue'
import FooterBar from './components/Footer.vue'


export default {
  name: 'app',
  components: {
    NavMenu,
    FooterBar
    
  },
  data() {
    return {  
    }
  },
  created() {
    this.$router.options.routes.forEach((page) => {
      this.pages.push(page.name)
    })
  }
}
</script>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Rubik:wght@300;400;600&display=swap');
  @import url('https://cdn.jsdelivr.net/npm/bootstrap@4.3.1/dist/css/bootstrap.min.css');

  * {
    font-family: 'Rubik', sans-serif;
  }
  .wrapper {
    margin: 0 60px;
    margin-top: 120px;
  }
  input {
    border-radius: 5px;
    border: 1px solid #eaeaea;
    transition: 0.2s border ease-in-out;
    padding: 10px 20px;
    min-width: 300px;
    height: 50px;
  }
  input:focus {
    border: 1px solid #282828;
    outline: none;
  }
  button {
    height: 50px;
    background: #282828;
    color: white;
    padding: 0 20px;
    border: none;
  }
</style>
