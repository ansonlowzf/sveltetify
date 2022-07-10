<script>
	import AnimationButton from '$lib/AnimationButton.svelte';
	import Container from '$lib/Container.svelte';
	import LinkHoverAnimation from '$lib/LinkHoverAnimation.svelte';
</script>

<Container>
	<h1>Welcome to SvelteKit</h1>
	<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>

	<LinkHoverAnimation />

	<AnimationButton />
</Container>
