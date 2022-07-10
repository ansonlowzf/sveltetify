<button>Contact Us</button>

<style>
	button {
		height: 50px;
		padding: 10px 30px;
		background-color: #199bed;
		color: #0f292f;
		font-size: 1rem;
		font-weight: 700;
		border: none;
		border-radius: 360px;
		box-shadow: rgba(0, 0, 0, 1) 4px 8px 4px;
		animation: shake 5.25s infinite;
		animation-timing-function: linear;
		cursor: pointer;
	}

	@keyframes shake {
		45% {
			transform: rotate(0deg);
		}
		50% {
			transform: rotate(-3deg);
		}
		55% {
			transform: rotate(3deg);
		}
		60% {
			transform: rotate(0deg);
		}
	}
</style>
