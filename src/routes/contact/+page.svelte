<script>
	import Title from '$lib/components/Title.svelte';
</script>

<main>
	<h1><Title title="contact" /></h1>

	<p>This is your contact page.. it can have a contact form or a link to your email.</p>

	<form action="">
		<legend>
			<label for="name">Name:</label>
			<input type="text" id="name" name="name" required />

			<label for="email">Email:</label>
			<input type="email" id="email" name="email" required />

			<label for="message">Message:</label>
			<textarea id="message" name="message" required></textarea>

			<button type="submit">Submit</button>
		</legend>
	</form>
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

	legend {
		display: flex;
		flex-direction: column;
		align-items: center;
		border: 1px solid black;
		border-radius: 10px;
		padding: 2rem;
		width: 25%;
		margin: 0 0 1% 37%;
		background: #ccc;
	}

	input {
		border-radius: 10px;
		margin-bottom: 2rem;
		border: none;
	}

	textarea {
		border-radius: 10px;
		margin-bottom: 2rem;
		border: none;
	}

	button {
		border-radius: 10px;
		padding: 1rem 2.5rem;
		background: #333;
		color: white;
		border: none;
		cursor: pointer;
		margin-top: 2rem;
	}
</style>
