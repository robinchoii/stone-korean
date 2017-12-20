<template>

	<div id="app" class='container'>

        <nav-bar></nav-bar>

		<full-menu></full-menu>

	</div>

</template>

<script>

	import FullMenu from './components/FullMenu.vue'
	import NavBar from './components/NavBar.vue'

	export default {

		name: 'app',

		components: {

			FullMenu, NavBar

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
