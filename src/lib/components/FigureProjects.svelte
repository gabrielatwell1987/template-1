<script>
	export let src;
	export let alt;
	export let figcaption;
</script>

<main>
	<figure>
		<img {src} {alt} />

		<!-- {#if figcaption} -->
		<figcaption>{figcaption}</figcaption>
		<!-- {/if} -->
	</figure>
</main>

<style>
	main {
		display: grid;
		grid-template-columns: repeat(3, minmax(100%, 5fr));
		place-items: center;
		position: relative;
		top: 0;
		left: -35%;
	}

	img {
		max-width: 100%;
		width: 26rem;
		border-radius: 1rem;
		margin: 10rem 3rem 2rem 0;
		object-fit: cover;
	}

	figure {
		position: relative;
		margin-right: 5rem;
	}

	figcaption {
		position: absolute;
		bottom: 2rem;
		background-color: rgba(0, 0, 0, 0.5);
		color: white;
		padding: 0.25rem 1rem;
		text-align: center;
		font-weight: 100;
		width: 89.5%;
		width: '{width}';
		border-bottom-right-radius: 1rem;
		border-bottom-left-radius: 1rem;
	}
</style>
