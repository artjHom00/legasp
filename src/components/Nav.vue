<template>
    <nav>
      <img src="../assets/gasp.png" width="80" alt="logo"/>
    </nav>
</template>

<script>
  import Vue from 'vue'

  export default Vue.extend({
    name: 'NavMenu',
    props: ["pages"],
    data() {
      return {
        activeIndex: 'asd',
        activeIndex2: '1'
      }
    },
    methods: {
      handleSelect(key, keyPath) {
        console.log(key, keyPath);
      }
    },

  })
</script>

<style>
  nav {
    margin: 30px 60px;
  }
</style>