<template>
	<p>{{ msg }}</p>
</template>

<script>
export default {
	name: "GreetingItem",
	data() {
		return {
			msg: "Hello World!",
		};
	},
};
</script>

<style scoped lang="scss">
$color: hsl(0deg, 100%, 50%);

p {
	color: $color;
}
</style>
