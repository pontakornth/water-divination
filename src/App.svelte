<script>
import Divination from './components/Divination.svelte';
</script>

<main>
	<Divination />
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 500px;
		margin: auto;
	}
	@media (min-width: 680px) {
		main {
			max-width: none;
		}
	}
</style>