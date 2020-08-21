<script>
	// import Nav from '../components/Nav.svelte';
	import Sidebar from '../components/Sidebar.svelte';

	// export let segment;
</script>

<style>
	main {
		display: grid;
		grid-template-columns: 1fr;
		place-content: flex-start;
		min-height: 100vh;
		flex-direction: column;
		background: var(--proposales-bg);
	}

	@media (min-width: 400px) {
		main {
			grid-template-columns: auto 1fr;
		}
	}
</style>

<!-- <Nav {segment}/> -->


<main>
	<Sidebar />
	<slot></slot>
</main>