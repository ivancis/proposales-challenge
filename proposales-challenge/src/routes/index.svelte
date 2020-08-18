<script>
	import Card from '../components/Card.svelte';
</script>

<style>
.page {
	margin: 0 auto;
	padding: 1em;
	width: 100%;
	max-width: var(--proposales-col-size);
}
</style>

<svelte:head>
	<title>Proposales : New proposal</title>
</svelte:head>

<div class="page">
	<div class="page-title">
		<h1>Create new proposal:</h1>
		<h3>Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. Cum sociis natoque penatibus et.</h3>
	</div>
	
	<div class="page-content">
		<ul class="card-list">
			<li class="card-list__item">
				<Card />
			</li>
			<li class="card-list__item">
				<Card />
			</li>
			<li class="card-list__item">
				<Card />
			</li>
			<li class="card-list__item">
				<Card />
			</li>
		</ul>
	</div>

	<div class="page-action">
	</div>
</div>
