<template>

	<div id="app" class=''>

        <nav-bar></nav-bar>

		<full-menu></full-menu>

		<google-map name='stonee'> </google-map>

		<!-- <food-picture></food-picture> -->
	</div>

</template>

<script>

	import FullMenu from './components/FullMenu.vue'
	import NavBar from './components/NavBar.vue'
	import FoodPicture from './components/FoodPicture.vue'
	import GoogleMap from './components/GoogleMap.vue'

	export default {

		name: 'app',

		components: {

			FullMenu, NavBar,FoodPicture, GoogleMap

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
