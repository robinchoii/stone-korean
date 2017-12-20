<template>

  <div id="app" class='container'>

    <nav-bar></nav-bar>

    <lunch-menu ></lunch-menu>

    <appetizers-menu> </appetizers-menu>

  </div>

</template>

<script>
    import NavBar from './components/NavBar.vue'
    import LunchMenu from './components/LunchMenu.vue'
    import AppetizersMenu from './components/AppetizersMenu.vue'

    export default {

        name: 'app',

        components: {

            NavBar, LunchMenu, AppetizersMenu

        },

        data () {

            return {

                msg: 'Stone Korean Restaurant',

            }

        }

    }

</script>

<style>
  #app {

    /*border: solid 1px black;*/

  }
</style>
