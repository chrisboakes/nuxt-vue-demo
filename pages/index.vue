<template>
	<div>
		<h1>Home Page</h1>
		<h2>This page is server-side rendered</h2>
		<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed tempor finibus ligula quis facilisis. Sed eget enim turpis. Mauris eget orci ligula. Duis in nisl consequat, iaculis lorem id, aliquam lorem. Nam mattis, orci a finibus tempor, tellus magna dictum velit, a porttitor massa ante et ante. Etiam lobortis nisi at commodo laoreet. Donec vitae dui non ligula tristique aliquet pharetra sed felis. In hac habitasse platea dictumst. Nulla condimentum sem vitae magna ultrices ultricies. Integer efficitur finibus nibh in pulvinar. Fusce suscipit faucibus laoreet. Duis lacus odio, aliquet ac pretium in, efficitur sagittis lectus. In malesuada orci nunc, non dignissim justo tincidunt eu.</p>
		<p>Duis egestas quam vitae nulla pellentesque, ac scelerisque magna maximus. Proin et lectus vitae nunc vehicula interdum. Praesent elit ipsum, porta a sem at, porttitor euismod lectus. Suspendisse congue ultricies odio, quis auctor nibh egestas eget. Etiam et mi at nunc rutrum efficitur. Mauris sem quam, tempor eget libero non, rhoncus posuere quam. Morbi interdum, velit scelerisque ultrices auctor, ante turpis aliquet mauris, id consequat mauris odio eget nulla. Nullam purus leo, congue quis tellus id, mattis faucibus elit. Nullam nec nulla pharetra odio iaculis eleifend. Nulla maximus, ante ut dapibus iaculis, felis justo ullamcorper lectus, eget tempor orci magna id mauris. Quisque ante sapien, interdum aliquet ligula a, semper fermentum turpis. Nam tincidunt efficitur quam a euismod.</p>
		<p>Morbi malesuada turpis at arcu placerat iaculis. Maecenas est urna, sollicitudin vitae leo ut, aliquet luctus erat. Ut lectus lectus, rutrum eu porta vitae, maximus ut lorem. Fusce quis consequat arcu. Integer consequat porttitor mauris in condimentum. Aenean non lacus eget sapien vulputate ornare. Sed mauris mi, pharetra auctor magna eget, tempus semper justo.</p>
		<p>Duis porta libero vitae turpis semper, eu cursus lorem dictum. Proin tincidunt, leo quis iaculis faucibus, nulla nibh hendrerit felis, et ultricies erat purus ac ligula. In et quam non dolor eleifend feugiat eget sit amet magna. Morbi dignissim hendrerit tortor at auctor. Vestibulum rutrum ante et semper fringilla. Integer accumsan egestas orci. Sed at arcu auctor, sagittis velit in, vulputate nunc. Aliquam consectetur mollis pretium. Mauris vitae blandit dolor.</p>
	</div>
</template>

<script>
export default {
	data () {
		return {
			title: 'Home'
		}
	},

	head () {
		return {
			title: this.title
		}
	}
}
</script>


