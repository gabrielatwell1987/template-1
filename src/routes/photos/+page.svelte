<script>
	import Photos from '$lib/components/Photos.svelte';
	import Title from '$lib/components/Title.svelte';
</script>

<h1><Title title="photos" /></h1>

<main>
	<div class="grid">
		<Photos
			src="https://images.pexels.com/photos/18156147/pexels-photo-18156147/free-photo-of-woman-wearing-wedding-dress-sitting-on-concrete-block.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1"
			alt="test"
			figcaption="woman in white dress"
		/>

		<Photos
			src="https://images.pexels.com/photos/15045040/pexels-photo-15045040/free-photo-of-man-standing-on-a-beach-in-a-suit.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1"
			alt="test"
			figcaption="a man in a suit"
		/>

		<Photos
			src="https://images.pexels.com/photos/20780434/pexels-photo-20780434/free-photo-of-a-blue-house-with-pink-blossoms-on-the-roof.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1"
			alt="test"
			figcaption="a house with pink blossoms"
		/>

		<Photos
			src="https://images.pexels.com/photos/21430836/pexels-photo-21430836/free-photo-of-vintage-camera-praktica-mtl5-hanging-on-the-strap-of-the-case.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1"
			alt="test"
			figcaption="a vintage camera"
		/>

		<Photos
			src="https://images.pexels.com/photos/21821150/pexels-photo-21821150/free-photo-of-a-black-and-white-photo-of-a-boat-on-a-lake.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1"
			alt="test"
			figcaption="a boat on a lake"
		/>

		<Photos
			src="https://images.pexels.com/photos/20882950/pexels-photo-20882950/free-photo-of-young-woman-holding-a-plant.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1"
			alt="test"
			figcaption="a woman holding a plant"
		/>
	</div>
</main>

<style>
	h1 {
		text-align: center;
		margin: 3rem 0 0 5%;
	}

	.grid {
		display: grid;
		grid-template-columns: repeat(3, 1fr);
		margin-left: 25rem;
	}
</style>
