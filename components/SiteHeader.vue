<template>
	<header>
		<Logo />
		<Navigation />
	</header>
</template>

<style>
	header {
		border-bottom: 1px solid grey;
		display: grid;
		grid-template-columns: repeat(12,1fr);
		padding: 20px;
	}
</style>

<script>
import Logo from '~/components/Logo.vue'
import Navigation from '~/components/Navigation.vue'

export default {
	components: {
		Logo,
		Navigation
	}
}
</script>
