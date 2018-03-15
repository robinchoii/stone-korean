<template>

	<div id="app" class=''>

        <nav-bar class='component' ></nav-bar>

		<nav-tabs class=''>

			<nav-tab name='Home' :selected='true'>

				<h1>Home</h1>

			</nav-tab>

			<nav-tab name='Photos'>

				<image-gallery></image-gallery>

			</nav-tab>

			<nav-tab name='Full Menu'>

				<full-menu></full-menu>

			</nav-tab>

			<nav-tab name='Lunch Specials'>

				<lunch-menu></lunch-menu>

			</nav-tab>

			<nav-tab name='Appetizers'>

				<appetizers-menu></appetizers-menu>

			</nav-tab>

			<nav-tab name='Soft Tofu Soups'>

				<soft-tofu-soup-menu></soft-tofu-soup-menu>

			</nav-tab>

			<nav-tab name='BiBimBobs'>

				<bibimbob-menu></bibimbob-menu>

			</nav-tab>

			<nav-tab name='B.B.Q.'>

				<bbq-menu></bbq-menu>

			</nav-tab>

			<nav-tab name='Combo Specials'>

				<combo-specials></combo-specials>

			</nav-tab>

			<nav-tab name='Fried Chicken'>

				<fried-chicken-menu></fried-chicken-menu>

			</nav-tab>

			<nav-tab name='Sauteed Dishes'>

				<sauteed-dishes-menu></sauteed-dishes-menu>

			</nav-tab>


			<nav-tab name='Grilled Fish'>

				<grilled-fish-menu></grilled-fish-menu>

			</nav-tab>

		</nav-tabs>

		<google-map  class='component google-map' name='stone'> </google-map>

		<contact class='component contact' id='contact'></contact>
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
    import LunchMenu from './components/LunchMenu.vue'
    import AppetizersMenu from './components/AppetizersMenu.vue'
    import SoftTofuSoupMenu from './components/SoftTofuSoupMenu.vue'
    import BibimbobMenu from './components/BiBimBobMenu.vue'
    import BbqMenu from './components/BBQMenu.vue'
    import FriedChickenMenu from './components/FriedChickenMenu.vue'
    import GrilledFishMenu from './components/GrilledFishMenu.vue'
    import SauteedDishesMenu from './components/SauteedDishesMenu.vue'
    import ComboSpecials from './components/ComboSpecials.vue'
    import ImageGallery from './components/ImageGallery.vue'


	export default {

		name: 'app',

		components: {

			FullMenu,
			NavBar,
			FoodPicture,
			GoogleMap,
			Contact,
			NavTabs,
			NavTab,
			LunchMenu,
			AppetizersMenu,
			SoftTofuSoupMenu,
			BibimbobMenu,
			BbqMenu,
			FriedChickenMenu,
			GrilledFishMenu,
			SauteedDishesMenu,
			ComboSpecials,
			ImageGallery

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

	#app {
        background-color: #3d1b1b;
        color: #e2e2e2;
	}

</style>
