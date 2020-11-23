<script>
	import { counter } from "./store";
	console.log(counter);
</script>

<main>
	<div class="main">
		<span class="text">counter value: {$counter}</span>
	</div>
</main>

<style lang="scss">
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
		.text {
			font-size: 14px;
			color: red;
		}
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>