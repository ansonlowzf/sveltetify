<script>
	import { page } from '$app/stores';

	export const navlinks = [
		{ name: 'home', url: '/' },
		{ name: 'about', url: '/about' },
		{ name: 'blog', url: '/blog' },
		{ name: 'contact', url: '/contact' }
	];
</script>

<nav>
	<ul class=" underline-indicators">
		<li class:active={$page.url.pathname === '/'}>
			<a class="ff-sans-cond text-white " href="/">home</a>
		</li>
		<li class:active={$page.url.pathname === '/about'}>
			<a class="ff-sans-cond text-white " href="/about">about</a>
		</li>
		<li class:active={$page.url.pathname === '/blog'}>
			<a class="ff-sans-cond text-white " href="/blog">blog</a>
		</li>
		<li class:active={$page.url.pathname === '/contact'}>
			<a class="ff-sans-cond text-white " href="/contact">contact</a>
		</li>
	</ul>
</nav>

<style>
	/* border-bottom: 0.2rem solid hsl(var(--color-white) / 0); */
	nav {
		height: 100%;
		width: 250px;
		position: fixed;
		z-index: 9;
		padding-top: 8em;
		top: 0;
		right: 0;
		background-color: hsl(var(--color-dark));
		overflow-x: hidden;
		transition: 0.5s;
	}
	nav > ul {
		list-style: none;
	}
	ul > * {
		cursor: pointer;
		padding: 1rem;
		border: 0;
	}
	ul li:hover,
	ul li:focus {
		opacity: 0.5;
	}
	a {
		text-decoration: none;
		text-transform: uppercase;
		letter-spacing: var(--letter-spacing-2);
	}
	@media (min-width: 60rem) {
		nav {
			display: inline-block;
			position: inherit;
			overflow-y: hidden;
			width: inherit;
			height: 5rem;
			padding-top: 0;
		}
		ul {
			display: flex;
			gap: 1rem;
		}
		.underline-indicators > *:hover,
		.underline-indicators > *:focus {
			border-color: hsl(var(--color-white) / 0.5);
		}
		.active {
			color: hsl(var(--color-white) / 1);
			border-color: hsl(var(--color-white) / 1);
		}
	}
</style>
