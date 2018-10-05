<template>

	<div id="app" class=''>

        <nav-bar class='navbar-component'></nav-bar>

		<nav-tabs class='navtabs-component'>

			<!-- <nav-tab name='' :selected='true'>

				<image-gallery></image-gallery>

			</nav-tab>

			<nav-tab name='Full Menu'>


			</nav-tab> -->

		</nav-tabs>

		<div class='main'>
			<full-menu></full-menu>
		</div>



		<google-map  class='component google-map-component' name='stone'> </google-map>

		<contact class='component contact-component' id='contact'></contact>
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
    import Catering from './components/Catering.vue'


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
			ImageGallery,
			Catering

		},

		data () {

				return {

						msg: 'Stone Korean Restaurant',

				}

		}

	}

</script>

<style>
	.navbar-component {
		grid-area: header;
		background-color: #cccccc
	}
	.navtabs-component {
		grid-area: tabs
	}
	.main {
		grid-area: main-content
	}
	.google-map-component {
		grid-area: maps;
	}
	.contact-component {
		grid-area: contact;
	}

	#app {
		display: grid;
		grid-template-columns: auto 1fr;
		grid-template-areas:
			"header header "
			"tabs main-content "
			"maps maps "
			"contact contact ";
        background-color: #3d1b1b;
        color: #e2e2e2;
        height: 100%;
        letter-spacing:2px;
        font-family: 'Oswald', sans-serif;

	}

</style>
