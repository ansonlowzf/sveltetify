<div class="container"><slot /></div>

<style>
	/* .container {
		border: 5px solid salmon;
		width: 100%;
		max-width: 600px;
		padding: 0 1em;
		margin: 0 auto;
	} */

	.container {
		border: 5px solid salmon;
		width: min(100% - 2rem, 600px);
		margin-inline: auto;
	}
</style>
