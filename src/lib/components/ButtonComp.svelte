<script>
	import { Button } from '@sveltestrap/sveltestrap';

	export let title;
	export let href;
</script>

<div class="button">
	<Button color="primary" size="lg" {href}>{title}</Button>
</div>

<!-- <style>
	.button {
		display: flex;
		justify-content: center;
		align-items: center;
	}
</style> -->
