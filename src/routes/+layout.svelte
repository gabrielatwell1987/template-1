<script>
	import '../app.css';
	import Nav from '$lib/components/Nav.svelte';
</script>

<main>
	<section class="nav">
		<Nav />
	</section>
</main>

<slot />

<style>
	:global(body) {
		background: #f0f0f0;
		background: url('/logos/blob-scene.svg') no-repeat center center/cover fixed;
		font-family: 'Arial', sans-serif;
	}

	main {
		display: flex;
		justify-content: space-between;
		align-items: center;
		background-color: #f0f0f0;
		padding: 1rem;
	}

	.nav {
		display: flex;
		justify-content: flex-end;
		align-items: center;
		margin-right: 10rem;
		margin-top: 1rem;
		margin-bottom: 1rem;
	}
</style>
