<script>
	import Button from '../components/Button.svelte';
</script>

<style>
	.card {
		display: grid;
		grid-template-columns: Min(10em, 200px) 1fr;
		grid-gap: 1em;
		background-color: #fff;
		border-radius: 1em;
		overflow: hidden;
	}

	.card-cover {
		position: relative;
		overflow: hidden;
		background: var(--proposales-medium);
	}
	
	.card-cover::before {
		display: block;
		content: "";
		width: 100%;
		padding-top: 100%;		
	}
	
	.card-cover__content {
		position: absolute;
		top: 0;
		left: 0;
		right: 0;
		bottom: 0;
	}

	.card-content {
		display: grid;
		grid-gap: .8em;
		padding: 1.2em 1em;
	}

	.card-title {
		font-size: 1.2em;
	}

	.card-subtitle {
		color: var(--proposales-medium);
		font-size: .8em;
	}
</style>

<div class="card">
	<div class="card-cover">
		<div class="card-cover__content">
			<slot name="card-image"></slot>
		</div>
	</div>
	<div class="card-content">
		<div class="card-title">
			<slot name="card-title"></slot>
		</div>
		<div class="card-subtitle">
			<slot name="card-subtitle"></slot>
		</div>
		<div class="card-action">
			<slot name="card-action"></slot>
		</div>
	</div>
</div>
