<template>
	<nav>
		<ul>
			<li><a href='/'>Home</a></li>
			<li><a href='/politics'>Politics</a></li>
			<li><a href='/news'>News</a></li>
		</ul>
	</nav>
</template>

<style scoped>
	nav {
		height: 100%;
		grid-column: 5/12;
	}

	ul {
		align-items: center;
		display: flex;
		height: 100%;
		list-style: none;
		margin: 0;
		padding: 0;
	}

	li {
		margin-right: 10px;
		padding-right: 10px;
	}
</style>
