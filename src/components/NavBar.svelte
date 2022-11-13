<script context="module">
	export const prerender = true;
</script>

<script>
  import { Navbar, NavBrand, NavHamburger, NavLi, NavUl, Button } from "flowbite-svelte";
</script>

<Navbar navClass="nav-bar" let:hidden let:toggle>
	<NavBrand href="/">
		<img
			src="/Calypso.svg"
			class="mr-9 h-12 sm:h-15"
			alt="Defund Logo"
		/>
	</NavBrand>
	<NavHamburger on:click={toggle} />
	<NavUl {hidden}>
		<button class="connect-but" color="light">Connect Wallet</button>
	</NavUl>
</Navbar>

<style>
  .nav-bar {
    background-color: black;
  }
  .connect-but {
	background-color: white;
    color: black;
    padding: 10px;
    border-radius: 10px;
    margin-right: 10px;
    width: 150px;
	height: 50px;
	font-weight: 500;
	font-size: 16px;
    font-family: inherit
  }
  .connect-but:hover {
	background-color: black;
    color: white;
  }
</style>
