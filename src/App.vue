<template>

	<div id="app" class='container'>

		<full-menu></full-menu>

	</div>

</template>

<script>

		import FullMenu from './components/FullMenu.vue'

		export default {

				name: 'app',

				components: {

					FullMenu

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
