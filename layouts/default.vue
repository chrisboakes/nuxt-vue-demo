<template>
	<div class="container">
		<SiteHeader />
		<main>
			<nuxt />
		</main>
	</div>
</template>

<style>
	main {
		position: relative;
		max-width: 56em;
		background-color: white;
		padding: 2em;
		margin: 0 auto;
		box-sizing: border-box;
	}
</style>

<script>
import SiteHeader from '~/components/SiteHeader.vue'

export default {
	components: {
		SiteHeader
	}
}
</script>
