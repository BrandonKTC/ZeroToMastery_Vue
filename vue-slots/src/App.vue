<template>
	<app-form>
		<template v-slot:help>
			<p>{{ help }}</p>
		</template>
		<template v-slot:fields>
			<input type="text" placeholder="email" />
			<input type="text" placeholder="username" />
			<input type="password" placeholder="password" />
		</template>
		<template v-slot:buttons>
			<button type="submit" @click.prevent>Submit</button>
		</template>
		<p>Dummy text</p>
	</app-form>
	<br />
	<app-form>
		<template v-slot:help>
			<p>Contact help text.</p>
		</template>
		<template v-slot:fields>
			<input type="text" placeholder="email" />
			<input type="text" placeholder="username" />
		</template>
		<template v-slot:buttons>
			<button type="submit" @click.prevent>Submit</button>
		</template>
	</app-form>
</template>

<script>
	import AppForm from '@/components/Form.vue'

	export default {
		name: 'App',
		components: {
			AppForm,
		},
		data() {
			return {
				help: 'This is some help text.',
			}
		},
	}
</script>
