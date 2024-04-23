<script>
	import Projects from '$lib/components/Projects.svelte';
	import Title from '$lib/components/Title.svelte';
</script>

<h1><Title title="projects" /></h1>

<main>
	<div class="one">
		<a href="https://google.com">
			<Projects
				src="https://images.pexels.com/photos/20350952/pexels-photo-20350952/free-photo-of-great-blue-heron-600mm-4x5.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1"
				alt=""
				figcaption="bird"
			/>
		</a>
	</div>

	<div class="two">
		<a href="https://google.com">
			<Projects
				src="https://images.pexels.com/photos/14119174/pexels-photo-14119174.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1"
				alt=""
				figcaption="bridge"
			/>
		</a>
	</div>

	<div class="three">
		<a href="https://google.com">
			<Projects
				src="https://images.pexels.com/photos/8570665/pexels-photo-8570665.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1"
				alt=""
				figcaption="crew only"
			/>
		</a>
	</div>

	<div class="four">
		<a href="https://google.com">
			<Projects
				src="https://images.pexels.com/photos/19059897/pexels-photo-19059897/free-photo-of-kitesurfing-on-sea-shore.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1"
				alt=""
				figcaption="ocean"
			/>
		</a>
	</div>

	<div class="five">
		<a href="https://google.com">
			<Projects
				src="https://images.pexels.com/photos/21656197/pexels-photo-21656197/free-photo-of-hot-air-balloons-flying-over-the-desert-in-egypt.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1"
				alt=""
				figcaption="parachutes"
			/>
		</a>
	</div>
</main>

<style>
	main {
		position: relative;
		margin-top: 10rem;
		margin-bottom: 5rem;
	}

	h1 {
		text-align: center;
		margin: 5rem 0 -10rem 0;
	}

	.one {
		position: absolute;
		top: 0;
		left: 20rem;
	}

	.two {
		position: absolute;
		top: 20rem;
		right: -60%;
	}

	.three {
		position: absolute;
		top: 40rem;
		left: 20rem;
	}

	.four {
		position: absolute;
		top: 60rem;
		right: -60%;
	}

	.five {
		position: absolute;
		top: 80rem;
		left: 20rem;
	}
</style>
