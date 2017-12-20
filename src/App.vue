<template>

	<div id="app" class='container'>

		<nav-bar></nav-bar>

		<lunch-menu ></lunch-menu>

		<appetizers-menu> </appetizers-menu>

		<soft-tofu-soup-menu></soft-tofu-soup-menu>

		<bibimbob-menu></bibimbob-menu>

		<bbq-menu></bbq-menu>

		<fried-chicken-menu></fried-chicken-menu>

		<grilled-fish-menu></grilled-fish-menu>

	</div>

</template>

<script>
		import NavBar from './components/NavBar.vue'
		import LunchMenu from './components/LunchMenu.vue'
		import AppetizersMenu from './components/AppetizersMenu.vue'
		import SoftTofuSoupMenu from './components/SoftTofuSoupMenu.vue'
		import BibimbobMenu from './components/BiBimBobMenu.vue'
		import BbqMenu from './components/BBQMenu.vue'
		import FriedChickenMenu from './components/FriedChickenMenu.vue'
		import GrilledFishMenu from './components/GrilledFishMenu.vue'

		export default {

				name: 'app',

				components: {

						NavBar, LunchMenu, AppetizersMenu, SoftTofuSoupMenu, BibimbobMenu, BbqMenu, FriedChickenMenu, GrilledFishMenu

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

	.item-description {
		line-height: 1;
		font-size: .75em;
	}

	.item-price {
		color: black;
		font-size:.8em;
		font-weight: 600;
	}

	.item-title {
		font-weight: 600;
		line-height: 1;
		margin-bottom: 3px
	}
</style>
