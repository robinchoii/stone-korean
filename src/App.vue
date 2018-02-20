<template>

	<div id="app" class=''>

        <nav-bar></nav-bar>

		<full-menu></full-menu>

		<!-- <food-picture></food-picture> -->
	</div>

</template>

<script>

	import FullMenu from './components/FullMenu.vue'
	import NavBar from './components/NavBar.vue'
	import FoodPicture from './components/FoodPicture.vue'

	export default {

		name: 'app',

		components: {

			FullMenu, NavBar,FoodPicture

		},

		data () {

				return {

						msg: 'Stone Korean Restaurant',

				}

		}

	}

</script>

<style>

</style>
