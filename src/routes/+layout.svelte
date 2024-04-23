<script>
	import '../app.css';
	import Nav from '$lib/components/Nav.svelte';
	import Image from '$lib/components/Image.svelte';
</script>

<main>
	<div class="logo">
		<a href="/">
			<Image picture="/logos/test1.png" desc="logo" x="300" y="50" />
		</a>
	</div>

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

	.logo {
		margin-left: 10rem;
		align-items: baseline;
		transition: transform 0.3s;
	}

	.logo:hover {
		transform: scale(1.1);
	}
</style>
