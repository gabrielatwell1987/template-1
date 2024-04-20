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

	let isOpen = false;
</script>

<Nav pills>
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

	<!-- <Dropdown theme="dark">
		<DropdownToggle caret>Links</DropdownToggle>
		<DropdownMenu end>
			<DropdownItem header>Links</DropdownItem>
			<DropdownItem divider />
			<DropdownItem href="https://svelte.dev">Svelte</DropdownItem>
			<DropdownItem divider />
			<DropdownItem href="https://gsap.com">GSAP</DropdownItem>
			<DropdownItem divider />
			<DropdownItem href="https://web.dev">Web.dev</DropdownItem>
		</DropdownMenu>
	</Dropdown> -->

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

<style>
	b {
		font-size: 1.2rem;
		font-weight: 800;
		margin-right: 1rem;
		padding-left: 1rem;
		/* letter-spacing: 0.1rem; */
	}
</style>
