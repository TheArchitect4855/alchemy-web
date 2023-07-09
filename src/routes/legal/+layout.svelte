<script>
	import Footer from "../Footer.svelte";
	import HeroIcon from "../HeroIcon.svelte";
</script>

<main>
	<HeroIcon />
	<slot></slot>
</main>
<Footer />

<style>
	main {
		margin: 5rem auto;
		max-width: 50ch;
		min-height: calc(100vh - 5rem);
		padding: 0 16px;
		text-align: center;
	}

	main :global(p) {
		text-align: justify;
	}
</style>
