<template>
    <div>
        <h6>Websites that sell your product!</h6>
        <h1>We create unique and commercially <br> successful websites.</h1>
        <short-form></short-form>
    </div>
</template>
  
<script>

    import Vue from 'vue'
    import ShortForm from '../components/ShortForm.vue'
    export default Vue.extend({
        name: 'MainSection',
        components: {
            ShortForm
        }
    })

</script>

<style>
    h1 {
        margin-bottom: 20px;
    }
</style>