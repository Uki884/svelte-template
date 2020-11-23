<script lang="ts">
	import { counter } from "./store";
	console.log(counter);
	
	const upCount = (): void=> {
		counter.update(n => n + 1)
	}
</script>

<main>
	<div class="main">
		<button class="text" on:click={() => upCount()}>counter value: {$counter}</button>
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