<script>
	import TwoLineHamburger from '$lib/TwoLineHamburger.svelte';
	import MainNav from './MainNav.svelte';
</script>

<header class="lg-container">
	<TwoLineHamburger width={48} />
	<MainNav />
</header>

<style>
	header {
		display: flex;
		justify-content: space-between;
		align-items: center;
		height: 5rem;
	}
</style>
