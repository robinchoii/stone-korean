<template>

  <div id="app" class='container'>

    <nav-bar></nav-bar>

    <lunch-menu ></lunch-menu>

    <appetizers-menu> </appetizers-menu>

    <soft-tofu-soup-menu></soft-tofu-soup-menu>

  </div>

</template>

<script>
    import NavBar from './components/NavBar.vue'
    import LunchMenu from './components/LunchMenu.vue'
    import AppetizersMenu from './components/AppetizersMenu.vue'
    import SoftTofuSoupMenu from './components/SoftTofuSoupMenu.vue'

    export default {

        name: 'app',

        components: {

            NavBar, LunchMenu, AppetizersMenu, SoftTofuSoupMenu

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

  .price {
    color: black;
  }
</style>
