<script lang="ts">
	let nnumbers = 10;
	$: numbers = [...Array(nnumbers).keys()];
</script>

<a href="/">← Back</a>
<p>How many numbers?</p>
<input type="number" bind:value={nnumbers} />
<div class="container">
	{#each numbers as number}
		<div class="number box">{number}</div>
	{/each}
</div>

<style>
	.container {
		display: flex;
		flex-wrap: wrap;
	}
</style>
