<template>

  <div id="app" class='container'>

    <nav-bar></nav-bar>

    <lunch-menu ></lunch-menu>

  </div>

</template>

<script>
    import NavBar from './components/NavBar.vue'
    import LunchMenu from './components/LunchMenu.vue'

    export default {

        name: 'app',

        components: {

            NavBar, LunchMenu

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

    /*border: solid 1px black;*/

  }
</style>
