<script>
    import Table from "./Table.svelte";
</script>

<div class="total-div">
    <h3 class="faded-white">Total</h3>
    <h2 class="price-header">$2,502.45</h2>
</div>
<div>
    <Table />
</div>

<style>
	.price-header {
		color: white;
		font-weight: bold;
		font-size: 40px;
		text-align: left;
	}
	.faded-white {
		color: rgba(255, 255, 255, 0.493);
        font-weight: bold;
	}
	.total-div {
		margin-top: 15px;
	}
</style>