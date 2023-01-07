<script lang="ts">
	const alphabet = [
		'A',
		'B',
		'C',
		'D',
		'E',
		'F',
		'G',
		'H',
		'I',
		'J',
		'K',
		'L',
		'M',
		'N',
		'O',
		'P',
		'Q',
		'R',
		'S',
		'T',
		'U',
		'V',
		'W',
		'X',
		'Y',
		'Z'
	];

	let nletters = 26;

	$: letters = alphabet.slice(0, nletters);
</script>

<a href="/">← Back</a>

<p>How many letters would you like to see?</p>
<input type="number" bind:value={nletters} />

<div class="container">
	{#each letters as letter}
		<div class="letter box">{letter}</div>
	{/each}
</div>

<style>
	.container {
		display: flex;
		flex-wrap: wrap;
	}
</style>
