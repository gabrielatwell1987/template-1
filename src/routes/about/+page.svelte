<script>
	import Title from '$lib/components/Title.svelte';
	import OffCanvas from '$lib/components/OffCanvas.svelte';
	import Image from '$lib/components/Image.svelte';
</script>

<h1><Title title="about" /></h1>

<main>
	<p>
		This is your about page. You can include everything that is about you. Hobbys, interests,
		skills. You can also post a link to your resume or CV. You can also include social media links.
	</p>

	<p>You can also include testimonials and linkedIn links.</p>

	<div class="two">
		<Image picture="/logos/standing-3.svg" desc="logo" x="500" y="650" />
	</div>

	<div class="three">
		<OffCanvas />
	</div>
</main>

<style>
	h1 {
		text-align: right;
		margin: 10% 10rem 0 0;
	}

	p {
		margin: 2% 13% 0 auto;
		width: 50%;
		line-height: 1.75;
		text-align: right;
	}

	main {
		position: relative;
		margin: 6% 0 0 0;
	}

	.two {
		position: absolute;
		top: -100%;
		left: 6%;
		max-width: 100%;
		margin: -5% 0 0 0;
	}

	.three {
		position: absolute;
		top: 200%;
		right: 12%;
		transform: translate(-20%, -200%);
		margin-top: 3%;
	}
</style>
