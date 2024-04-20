<script>
	import { Button, Offcanvas } from '@sveltestrap/sveltestrap';

	let isOpen = false;

	const toggle = () => {
		isOpen = !isOpen;
	};
</script>

<Button color="primary" on:click={toggle}>Open Me</Button>

<Offcanvas {isOpen} {toggle} backdrop={false}>
	<h2 slot="header">
		<i>Random</i> <b>stuff!</b>
	</h2>

	<h5>You can put random stuff here.. like pictures, links, videos, etc..</h5>
</Offcanvas>

<style>
	i {
		color: #007bff;
		font-size: 2.03rem;
	}

	b {
		color: #28a745;
		font-size: 2rem;
		font-weight: 700;
	}

	h5 {
		line-height: 2;
	}
</style>
