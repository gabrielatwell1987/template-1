<script>
	import Title from '$lib/components/Title.svelte';
</script>

<main>
	<h1><Title title="contact" /></h1>

	<p>This is your contact page.. it can have a contact form or a link to your email.</p>

	<p><a href="mailto:example@example.com">example@example.com</a></p>

	<img src="/logos/sitting-4.svg" alt="" />
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

	img {
		margin-top: -1rem;
	}
</style>
