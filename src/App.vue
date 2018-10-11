<template>

	<div id="app" class=''>

        <nav-bar class='navbar'></nav-bar>

		<nav-tabs class='navtabs-container'>
			<nav-tab name="Home" :selected='true'>
				<overview></overview>
				<image-gallery></image-gallery>
			</nav-tab>
			<nav-tab name="Redmond">
				<full-menu></full-menu>
			</nav-tab>
			<nav-tab name="Seattle">
				<seattle-full-menu></seattle-full-menu>
			</nav-tab>
			<nav-tab name="Contact">
				<contact id='contact'></contact>
			</nav-tab>
			<nav-tab name='Order Online'>
				<order-online></order-online>
			</nav-tab>
		</nav-tabs>

		<section class='google-maps-container'>
			<google-map name='stone'> </google-map>
		</section>
		<section class='contact-container'>
		</section>
	</div>

</template>

<script>
	import FullMenu from './components/FullMenu.vue'
	import NavBar from './components/NavBar.vue'
	import GoogleMap from './components/GoogleMap.vue'
	import Contact from './components/Contact.vue'
	import NavTabs from './components/Navtabs.vue'
	import NavTab from './components/Navtab.vue'
    import ImageGallery from './components/ImageGallery.vue'
    import Catering from './components/Catering.vue'
    import Overview from './components/Overview.vue'
    import OrderOnline from './components/OrderOnline.vue'
    import SeattleFullMenu from './components/Seattle/SeattleFullMenu.vue'

	export default {

		name: 'app',

		components: {

			FullMenu,
			NavBar,
			GoogleMap,
			Contact,
			NavTabs,
			NavTab,
			ImageGallery,
			Catering,
			Overview,
			SeattleFullMenu,
			OrderOnline
		},

		data () {

				return {

						msg: 'Stone Korean Restaurant',

				}

		}

	}

</script>

<style>
	.navbar {
		grid-area: header;
		background-color: #cccccc;
		padding: 10px 0 10px 0;
	}
	.navtabs-container {
		grid-area: tabs;
	}
	.image-gallery-container {
		grid-area: gallery;
	}
	.google-maps-container {
		grid-area: maps;
	}
	.contact-container {
		grid-area: contact;
	}
	#app {
		display: grid;
		grid-template-columns: auto 3fr	1fr;
		grid-template-areas:
			"header header header"
			"tabs tabs tabs"
			"maps maps maps"
			"contact contact contact";
        background-color: #3d1b1b;
        color: #e2e2e2;
        height: 100%;
        letter-spacing:2px;
        font-family: 'Oswald', sans-serif;

	}
</style>
