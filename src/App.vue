<template>

	<div id="app" class=''>

        <nav-bar class='component' ></nav-bar>

        <!-- <left-nav></left-nav> -->

		<full-menu class='component' ></full-menu>

		<contact class='component contact'></contact>

		<google-map  class='component' name='stone'> </google-map>
		<!-- <food-picture></food-picture> -->
	</div>

</template>

<script>

	import FullMenu from './components/FullMenu.vue'
	import NavBar from './components/NavBar.vue'
	import FoodPicture from './components/FoodPicture.vue'
	import GoogleMap from './components/GoogleMap.vue'
	import Contact from './components/Contact.vue'
	import LeftNav from './components/LeftNav.vue'

	export default {

		name: 'app',

		components: {

			FullMenu, NavBar,FoodPicture, GoogleMap, Contact, LeftNav

		},

		data () {

				return {

						msg: 'Stone Korean Restaurant',

				}

		}

	}

</script>

<style>
	.component {
		/*border: 2px solid green;*/
	}

</style>
