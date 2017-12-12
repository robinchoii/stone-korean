<template>

  <div id="app" class='container'>

    <NavBar></NavBar>

  </div>

</template>

<script>
    import NavBar from './components/NavBar.vue'

    export default {

        name: 'app',

        components: {

            NavBar

        },

        data () {

            return {

            msg: 'Stone Korean Restaurant'

            }

        }

    }

</script>

<style>
  #app {

    border: solid 1px black;

  }
</style>
