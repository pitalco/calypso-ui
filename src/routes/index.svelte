<script context="module">
	export const prerender = true;
</script>

<script>
	import Assets from "../components/Assets.svelte";
	import Trade from "../components/Trade.svelte";
	import Liquidity from "../components/Liquidity.svelte";
	import Staking from "../components/Staking.svelte";
	import { ButtonGroup, ButtonGroupItem } from 'flowbite-svelte';

	let AssetDisplay = "block"
	let TradeDisplay = "none"
	let LiquidityDisplay = "none"
	let StakingDisplay = "none"

	let btnTabClassAsset = AssetDisplay == "block" ? "bg-black-active" : "bg-black"
	let btnTabClassTrade = TradeDisplay == "block" ? "bg-black-active" : "bg-black"
	let btnTabClassLiquidity = LiquidityDisplay == "block" ? "bg-black-active" : "bg-black"
	let btnTabClassStaking = StakingDisplay == "block" ? "bg-black-active" : "bg-black"

	function changeTab(tab = "assets") {
		tab == "assets" ? AssetDisplay = "block" : AssetDisplay = "none"
		tab == "trade" ? TradeDisplay = "block" : TradeDisplay = "none"
		tab == "assets" ? LiquidityDisplay = "block" : LiquidityDisplay = "none"
		tab == "trade" ? StakingDisplay = "block" : StakingDisplay = "none"

		btnTabClassAsset = AssetDisplay == "block" ? "bg-black-active" : "bg-black"
		btnTabClassTrade = TradeDisplay == "block" ? "bg-black-active" : "bg-black"
		btnTabClassLiquidity = LiquidityDisplay == "block" ? "bg-black-active" : "bg-black"
		btnTabClassStaking = StakingDisplay == "block" ? "bg-black-active" : "bg-black"
	}
</script>

<svelte:head>
	<title>Dashboard</title>
	<meta name="Calypso" content="The Crypto Terminal" />
</svelte:head>

<section>
	<div>
		<ButtonGroup>
			<ButtonGroupItem on:click={() => changeTab("assets")} btnClass="{btnTabClassAsset}">Assets</ButtonGroupItem>
			<ButtonGroupItem on:click={() => changeTab("trade")} btnClass="{btnTabClassTrade}">Trade</ButtonGroupItem>
			<ButtonGroupItem on:click={() => changeTab("liquidity")} btnClass="bg-black">Liquidity</ButtonGroupItem>
			<ButtonGroupItem on:click={() => changeTab("staking")} btnClass="bg-black">Staking</ButtonGroupItem>
		</ButtonGroup>

		<div style="display: {AssetDisplay};"><Assets/></div>
		<div style="display: {TradeDisplay};"><Trade/></div>
		<div style="display: {LiquidityDisplay};"><Liquidity/></div>
		<div style="display: {StakingDisplay};"><Staking/></div>
	</div>
</section>

<style>
</style>
