<template>
	<div>
		<h1>{{ post.title }}</h1>

		<h2>This page is server-side rendered</h2>

		<p>{{ post.standfirst }}</p>

		<div class='content' v-html="post.content"></div>
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

	fetchOnServer: true
}
</script>
