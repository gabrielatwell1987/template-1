<script>
	export let title;
</script>

<h1>{title}</h1>

<style>
	h1 {
		letter-spacing: 5rem;
		font-weight: 700;
	}

	@media (min-width: 300px) {
		h1 {
			letter-spacing: 1rem;
			text-align: center;
			margin-left: 55%;
		}
	}

	@media (min-width: 720px) {
		h1 {
			letter-spacing: 2.5rem;
			margin-left: 0.2%;
			font-size: 3rem;
		}
	}

	@media (min-width: 1024px) {
		h1 {
			letter-spacing: 5rem;
			margin-left: -10%;
			font-size: 5rem;
			font-weight: 800;
		}
	}
</style>
