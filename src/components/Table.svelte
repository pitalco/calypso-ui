<script context="module">
	export const prerender = true;
</script>

<script>
    // @ts-nocheck
    import SvelteTable from "svelte-table";
    import { goto } from '$app/navigation';
    /**
    * @type {Object[]}
    */
    const rows = [
        { asset: "ATOM", owned: 56, price: "$7.54", total: "$1,045" },
    ];
    /**
    * @type {Object[]}
    */
    const columns = [
        {
            key: "asset",
            title: "Asset",
            // @ts-ignore
            value: v => v.asset,
            sortable: true,
        },
        {
            key: "owned",
            title: "Owned",
            // @ts-ignore
            value: v => v.owned,
            sortable: true,
        },
        {
            key: "price",
            title: "Price",
            // @ts-ignore
            value: v => v.price,
            sortable: true,
        },
        {
            key: "total",
            title: "Total",
            // @ts-ignore
            value: v => v.total,
            sortable: true,
        }
    ];
</script>

<div class="table-div">
    <SvelteTable
        columns="{columns}"
        rows="{rows}"
    >
    </SvelteTable>
</div>

<style>
	.table-div {
        margin-top: 15px;
        margin-bottom: 15px;		
	}
</style>