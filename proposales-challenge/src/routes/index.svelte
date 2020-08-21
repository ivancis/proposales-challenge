<script>
	import Button from '../components/Button.svelte';
	import Card from '../components/Card.svelte';
</script>

<style>
	.page {
		display: grid;
		grid-gap: 1em;
		place-content: flex-start;
		margin: 0 auto;
		padding: 1em 1.5em;
		width: 100%;
		max-width: var(--proposales-col-size);
	}

	.page-head {
		display: grid;
		/* REVIEW */
		grid-template-columns: 1fr auto;
	}
	
	.proposal-build {
		display: grid;
		/* REVIEW */
		grid-template-columns: 1fr 1fr;
		grid-gap: 2em;
	}

	.proposal-build__products-list {
		display: grid;
		grid-gap: 1em;
	}

	/* REVIEW */
	.card-image > *{
		object-fit: cover;
		height: 100%;
	}
</style>

<svelte:head>
	<title>Proposales : New proposal</title>
</svelte:head>

<div class="page">
	<div class="page-head">
		<div class="page-head__title">
			<h1>Create new proposal:</h1>
			<h3>Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. Cum sociis natoque penatibus et.</h3>
		</div>
		<div class="page-head__action">
			<Button>Save proposal</Button>
		</div>
	</div>
	
	<div class="page-content">
		<div class="proposal-build">
			<ul class="proposal-build__products-list">
				<li class="proposal-build__product-item">
					<Card>
						<span class="card-image" slot="card-image">
							<img src="https://images.unsplash.com/photo-1519494026892-80bbd2d6fd0d?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1335&q=80">
						</span>
						<span slot="card-title">Intro</span>
						<span slot="card-subtitle">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptatibus quia.</span>
						<span slot="card-action">
							<Button
								variant="hollow"
								size="small"
							>
								Add Intro
							</Button>
						</span>
					</Card>
				</li>
				<li class="proposal-build__product-item">
					<Card>
						<span class="card-image" slot="card-image">
							<img src="https://images.unsplash.com/photo-1571624436279-b272aff752b5?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1352&q=80">
						</span>
						<span slot="card-title">Meeting room</span>
						<span slot="card-subtitle">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptatibus quia.</span>
						<span slot="card-action">
							<Button
								variant="hollow"
								size="small"
							>
								Add meeting
								 room</Button>
						</span>
					</Card>
				</li>
				<li class="proposal-build__product-item">
					<Card>
						<span class="card-image" slot="card-image">
							<img src="https://images.unsplash.com/photo-1498837167922-ddd27525d352?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1350&q=80">
						</span>
						<span slot="card-title">Food & Beverage</span>
						<span slot="card-subtitle">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptatibus quia.</span>
						<span slot="card-action">
							<Button
								variant="hollow"
								size="small"
							>
								Add F&B
							</Button>
						</span>
					</Card>
				</li>
				<li class="proposal-build__product-item">
					<Card>
						<span slot="card-title">Upselling</span>
						<span slot="card-subtitle">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptatibus quia.</span>
						<span slot="card-action">
							<Button
								variant="hollow"
								size="small"
							>
								Add Upselling
							</Button>
						</span>
					</Card>
				</li>
			</ul>

			<div class="proposal-preview">
				hello preview
			</div>
		</div>
	</div>

	<div class="page-footer">
		<div class="page-footer__action">
			<Button>Save proposal</Button>
		</div>
	</div>
</div>
