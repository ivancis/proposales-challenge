<script>
	// import Nav from '../components/Nav.svelte';

	// export let segment;
</script>

<style>
	main {
		display: grid;
		min-height: 100vh;
		border-top: 1em solid var(--proposales-dark);
	}
</style>

<!-- <Nav {segment}/> -->

<main>
	<slot></slot>
</main>