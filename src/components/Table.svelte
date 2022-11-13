<script context="module">
	export const prerender = true;
</script>

<script>
    // @ts-nocheck
    import SvelteTable from "svelte-table";
    /**
    * @type {Object[]}
    */
    const rows = [
        { chain: "Osmosis", asset: "ATOM", owned: 56, price: "$7.54", total: "$1,045.00" },
        { chain: "Juno", asset: "JUNO", owned: 1, price: "$10.24", total: "$10.24" },
        { chain: "Secret", asset: "SCRT", owned: 100, price: "$0.64", total: "$64.00" },
    ];
    /**
    * @type {Object[]}
    */
    const columns = [
        {
            key: "chain",
            title: "Chain",
            // @ts-ignore
            value: v => v.chain,
            sortable: true,
        },
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