<script>
	import Title from '$lib/components/Title.svelte';
	import Image from '../../lib/components/Image.svelte';
</script>

<main>
	<h1><Title title="contact" /></h1>

	<p>This is your contact page.. it can have a contact form or a link to your email.</p>

	<p><a href="mailto:example@example.com">example@example.com</a></p>

	<!-- <img src="/logos/sitting-4.svg" alt="" /> -->
	<Image picture="/logos/sitting-4.svg" desc="logo" x="500" y="600" />
</main>

<style>
	main {
		text-align: center;
	}

	h1 {
		margin-top: 5%;
	}

	p {
		margin-top: 4%;
	}
</style>
