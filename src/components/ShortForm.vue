<template>
  <div>
    <form>
        <input placeholder="example@gmail.com" name="text" class="input" autocomplete="off"/>
        <button>Get free consultation</button>
    </form>
  </div>
</template>

<script>
import Vue from 'vue'

export default Vue.extend({
    name: 'shortForm',
})
</script>

<style>
    button {
        position: relative;
        left: -20px;
    }
</style>