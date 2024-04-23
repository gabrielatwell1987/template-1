<script>
	export let picture;
	export let desc;
	export let x;
	export let y;
</script>

<img src={picture} alt={desc} width={x} height={y} />

<style>
	img {
		object-fit: cover;
	}
</style>
