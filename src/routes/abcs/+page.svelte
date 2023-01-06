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
</script>

<a href="/">← Back</a>
<div class="container">
	{#each alphabet as letter}
		<div class="letter box">{letter}</div>
	{/each}
</div>

<style>
	.container {
		display: flex;
		flex-wrap: wrap;
	}
</style>
