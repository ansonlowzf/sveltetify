<nav class="navbar">
	<input type="checkbox" name="" id="menu-toggle" />
	<label for="menu-toggle" class="hamburger">
		<span class="bun bun-top">
			<span class="bun-crust bun-crust-top" />
		</span>
		<span class="bun bun-bottom">
			<span class="bun-crust bun-crust-bottom" />
		</span>
	</label>
</nav>

<style>
	#menu-toggle {
		display: none;
	}

	.hamburger {
		display: block;
		width: 4.8rem;
		height: 4.8rem;
		position: relative;
		cursor: pointer;
	}

	.bun {
		width: 3rem;
		height: 3rem;
		position: absolute;
		top: 0.9rem;
		left: 0.9rem;
		transition: transform 0.16s cubic-bezier(0.04, 0.04, 0.12, 0.96) 0.15s;
	}

	.bun-crust {
		display: block;
		width: 1.5rem;
		height: 1px;
		background-color: white;
		border-radius: 1px;
		position: absolute;
		left: 0.8rem;

		transition: transform 0.16s cubic-bezier(0.52, 0.16, 0.52, 0.84) 0.2s;
	}

	.bun-crust-top {
		top: 1.4rem;
		transform: translateY(-3px);
	}

	.bun-crust-bottom {
		bottom: 1.4rem;
		transform: translateY(3px);
	}

	#menu-toggle:checked + .hamburger .bun-top {
		transform: rotate(45deg);
	}

	#menu-toggle:checked + .hamburger .bun-bottom {
		transform: rotate(-45deg);
	}

	#menu-toggle:checked + .hamburger .bun-crust-top,
	#menu-toggle:checked + .hamburger .bun-crust-bottom {
		transform: none;
		transition: transform 0.18s cubic-bezier(0.04, 0.04, 0.12, 0.96);
	}
</style>
