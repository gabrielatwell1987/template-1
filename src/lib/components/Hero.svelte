<script>
	import Button from '$lib/components/ButtonComp.svelte';
	import Title from '$lib/components/Title.svelte';
	import Image from '$lib/components/Image.svelte';
</script>

<main>
	<div class="logo">
		<Image src="/logos/sitting-7.svg" alt="logo" width="700" height="800" />
	</div>

	<section class="hero">
		<h1><Title title="title" /></h1>

		<h2>Subtitle</h2>

		<p>
			this is the main content of your hero section. You can add a button here to direct users to
			another page. please note that the point of a hero section is to grab the user's attention and
			give them a brief overview of what your site is about.
		</p>

		<div class="button">
			<Button title="Projects" href="/projects" />
		</div>
	</section>
</main>

<style>
	main {
		display: flex;
		justify-content: space-between;
		align-items: center;
		background-color: #f0f0f0;
		padding: 1rem;
		position: relative;
		z-index: -1;
	}

	.logo {
		position: absolute;
		top: 1rem;
		right: 5%;
		max-width: 100%;
		min-width: 20rem;
		margin-top: 3%;
	}

	h1 {
		margin: 8% 0 -5% 13.5%;
	}

	h2 {
		margin: 5% 0 -6% 13.75%;
	}

	p {
		width: 45%;
		margin: 10rem 13.5%;
	}

	.button {
		display: flex;
		justify-content: flex-start;
		margin-top: -5rem;
		margin-left: 13.5%;
	}
</style>
