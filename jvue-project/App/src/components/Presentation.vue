<template>
	<section id="presentation" class="presentation">
		<p>{{ txtpresentation }}</p>
		<p>Made by {{ author }}</p>
	</section>
</template>

<script>
	export default{
		props: [
			'author',
			'txtpresentation'
		]
	}
</script>

<style scoped lang="scss">
	@import './src/assets/sass/main.scss'
</style>