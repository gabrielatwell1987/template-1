<script>
	import Title from '$lib/components/Title.svelte';
	import OffCanvas from '$lib/components/OffCanvas.svelte';
</script>

<h1><Title title="about" /></h1>

<main>
	<p>
		This is your about page. You can include everything that is about you. Hobbys, interests,
		skills. You can also post a link to your resume or CV. You can also include social media links.
	</p>

	<div class="two">
		<img src="/logos/standing-3.svg" height="650px" alt="" />
	</div>

	<div class="three">
		<OffCanvas />
	</div>
</main>

<style>
	img {
		max-width: 100%;
		margin: -20% 0 0 0;
	}

	h1 {
		text-align: right;
		margin: 5rem 10rem 0 0;
	}

	p {
		margin: 5% 10rem 0 auto;
		width: 50%;
		line-height: 2.75;
	}

	main {
		position: relative;
		margin: 6% 0 0 0;
	}

	.two {
		position: absolute;
		top: -100%;
		left: 6%;
		width: 50%;
	}

	.three {
		position: absolute;
		top: 200%;
		left: 89%;
		transform: translate(-89%, -200%);
	}
</style>
