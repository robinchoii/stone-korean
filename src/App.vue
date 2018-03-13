<template>

	<div id="app" class=''>

        <nav-bar class='component' ></nav-bar>

		<!-- <full-menu class='component' ></full-menu> -->
		<nav-tabs>

			<nav-tab name='Home' :selected='true'>

				<h1>Home</h1>

			</nav-tab>

			<nav-tab name='Full Menu'>

				<h1>Full Menu</h1>

			</nav-tab>

			<nav-tab name='Lunch Specials'>

				<h1>Lunch Specials</h1>

			</nav-tab>

			<nav-tab name='Appetizers'>

				<h1>Appetizers</h1>

			</nav-tab>

		</nav-tabs>

		<google-map  class='component' name='stone'> </google-map>

		<contact class='component contact'></contact>
		<!-- <food-picture></food-picture> -->
	</div>

</template>

<script>

	import FullMenu from './components/FullMenu.vue'
	import NavBar from './components/NavBar.vue'
	import FoodPicture from './components/FoodPicture.vue'
	import GoogleMap from './components/GoogleMap.vue'
	import Contact from './components/Contact.vue'
	import NavTabs from './components/Navtabs.vue'
	import NavTab from './components/Navtab.vue'

	export default {

		name: 'app',

		components: {

			FullMenu, NavBar,FoodPicture, GoogleMap, Contact, NavTabs, NavTab

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
