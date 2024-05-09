<script lang="ts">
	import {
		Nav,
		NavItem,
		Dropdown,
		DropdownItem,
		DropdownToggle,
		DropdownMenu,
		NavLink
	} from '@sveltestrap/sveltestrap';

	import Image from './Image.svelte';

	let isOpen = false;
</script>

<div class="nav">
	<div class="logo">
		<a href="/">
			<Image src="/logos/test1.png" alt="logo" width="300" height="50" />
		</a>
	</div>

	<Nav underline>
		<NavItem>
			<NavLink href="/about"><b>About</b></NavLink>
		</NavItem>

		<NavItem>
			<NavLink href="/projects"><b>Projects</b></NavLink>
		</NavItem>

		<NavItem>
			<NavLink href="/photos"><b>Photos</b></NavLink>
		</NavItem>

		<NavItem>
			<NavLink href="/contact"><b>Contact</b></NavLink>
		</NavItem>

		<Dropdown nav {isOpen} toggle={() => (isOpen = !isOpen)}>
			<DropdownToggle nav caret><b>Links</b></DropdownToggle>
			<DropdownMenu end>
				<DropdownItem href="https://svelte.dev">Svelte</DropdownItem>
				<DropdownItem divider />
				<DropdownItem href="https://gsap.com">GSAP</DropdownItem>
				<DropdownItem divider />
				<DropdownItem href="https://web.dev">Web.dev</DropdownItem>
			</DropdownMenu>
		</Dropdown>
	</Nav>
</div>

<style>
	b {
		font-size: 1.2rem;
		font-weight: 800;
		margin-right: 0.25rem;
		padding-left: 0.25rem;
	}

	.logo {
		margin-left: 55%;
		align-items: baseline;
		transition: transform 0.3s;
	}

	.logo:hover {
		transform: scale(1.1);
	}

	@media (min-width: 300px) {
		b {
			font-size: 1rem;
		}

		.nav {
			position: fixed;
			top: 1%;
			left: 5%;
			margin-bottom: 2rem;
			transform: scale(0.75);
		}

		.logo {
			margin-left: 12%;
		}
	}

	@media (min-width: 720px) {
		b {
			font-size: 1.75rem;
		}

		.nav {
			position: fixed;
			top: 1%;
			left: 2%;
			margin: 0 0 2rem auto;
			transform: scale(0.5);
		}

		.logo {
			margin-right: 20%;
		}
	}

	@media (min-width: 1024px) {
		b {
			font-size: 1.75rem;
		}

		.nav {
			position: fixed;
			top: 5%;
			left: 32%;
			margin-bottom: 2rem;
			transform: scale(1);
		}

		.logo {
			margin-left: 20%;
		}
	}
</style>
