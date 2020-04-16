<template>
	<div>
		<p v-if="$fetchState.pending">Fetching post...</p>
		
		<div v-else>
			<h1>{{ post.title }}</h1>

			<h2>This page is client side rendered</h2>

			<p>{{ post.standfirst }}</p>

			<div class='content' v-html="post.content"></div>
		</div>
	</div>
</template>

<script>
export default {
	data() {
		return {
			title: '',
			post: {}
		}
	},

	head () {
		return {
			title: this.title
		}
	},

	async fetch () {
		this.post = await fetch(`https://my-json-server.typicode.com/chrisboakes/nuxt-vue-demo/${this.$route.params.slug}`).then((response) => {
			return response.json()
		})

		this.title = this.post.title
	},

	fetchOnServer: false
}
</script>
