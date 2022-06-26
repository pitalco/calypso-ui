<script context="module">
	export const prerender = true;
</script>

<script>
	import Table from "../components/Table.svelte";
	import { ButtonGroup, ButtonGroupItem } from 'flowbite-svelte';
</script>

<svelte:head>
	<title>Dashboard</title>
	<meta name="Calypso" content="The Crypto Terminal" />
</svelte:head>

<section>
	<div>
		<ButtonGroup>
			<ButtonGroupItem btnClass="bg-black-active">Assets</ButtonGroupItem>
			<ButtonGroupItem btnClass="bg-black">Liquidity</ButtonGroupItem>
			<ButtonGroupItem btnClass="bg-black">Staking</ButtonGroupItem>
		</ButtonGroup>
		<div class="total-div">
			<h3 class="faded-white">Total</h3>
			<h2 class="price-header">$2,502.45</h2>
		</div>
		<div>
			<Table />
		</div>
	</div>
</section>

<style>
	.price-header {
		color: white;
		font-weight: bold;
		font-size: 40px;
		text-align: left;
	}
	.faded-white {
		color: rgba(255, 255, 255, 0.493);
	}
	.total-div {
		margin-top: 15px;
	}
</style>
