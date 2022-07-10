<ul class="list">
	<li><a href="/" class="link">Link 1</a></li>
	<li><a href="/" class="link">Link 2</a></li>
	<li><a href="/" class="link">Link 3</a></li>
</ul>

<style>
	.list {
		list-style: none;
	}

	.link {
		display: inline-block; /*By default, anchor tags will be display of inline. We change this behavior to inline-block so that it will allow for the use of margin top and bottom.*/
		margin-block: 2px;
		text-decoration: none;
		color: #fff;
		position: relative; /*Relative positioning is required for the pseudo-element we will create it since it will have position of absolute. */
	}

	.link::after {
		content: '';
		width: 100%;
		height: 1px;
		background-color: #fed86b;
		border-radius: 4px;
		position: absolute;
		left: 0;
		bottom: 0;
		transform: scaleX(0);
		transform-origin: left;
		transition: transform 0.25s ease;
	}

	.link:hover::after {
		transform: scaleX(1);
	}
</style>
