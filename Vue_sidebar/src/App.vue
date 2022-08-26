<template>
	<div id="app">
		<hello-world #default="{user, favorites}">
			<p>Hello {{user.name}}</p>
			<ul v-for="item in favorites">
				<li>
					{{ item }}
				</li>
			</ul>
		</hello-world>
	</div>
</template>

<script>
	import HelloWorld from './components/HelloWorld.vue'

	export default {
		name: 'App',
		components: {
			HelloWorld,
		},
	}
</script>
