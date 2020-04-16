<template>
	<div>
		<h1>Politics</h1>
		<h2>This page is server-side rendered</h2>
		<p v-if="$fetchState.pending">Fetching posts...</p>
		<p v-else-if="$fetchState.error">Error while fetching posts: {{ $fetchState.error.message }}</p>
		<ul v-else>
			<li v-for="post of posts">
				<n-link :to="`/${post.section}/${post.slug}`">{{ post.title }}</n-link>
			</li>
		</ul>
	</div>
</template>

<style scoped>
	a {
		text-decoration: underline;
	}
</style>

<script>
export default {
	data () {
		return {
			posts: []
		}
	},

	async fetch () {
		this.posts = await fetch('https://my-json-server.typicode.com/chrisboakes/nuxt-vue-demo/politics-articles').then((response) => {
			return response.json()
		})
	},

	fetchOnServer: true
}
</script>

