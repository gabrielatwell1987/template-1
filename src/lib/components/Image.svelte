<script>
	export let src;
	export let alt;
	export let width;
	export let height;
</script>

<img {src} {alt} {width} {height} />

<style>
	img {
		object-fit: cover;
	}
</style>
