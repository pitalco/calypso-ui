<script>
    import { Input } from "flowbite-svelte";
</script>

<div class="swap-main-div">
    <div class="swap-div">
        <Input type="number" value=0 size="lg"></Input>
        <Input type="number" value=0 size="lg"></Input>
        <button class="trade-button" color="light">Transfer</button>
    </div>
</div>

<style>
    .transfer-main-div {
        margin-top: 20px;
        padding: 30px;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-wrap: wrap;
    }
    .transfer-div {
        padding: 30px;
        background-color: white;
        max-width: 500px;
        border-radius: 15px;
        min-height: 350px;
        display: flex;
        justify-content: flex-start;
        flex-wrap: wrap;
        align-items: center;
        align-content: space-between;
    }
    .transfer-button {
        width: 100%;
        background-color: black;
        color: white;
        padding: 15px;
        border-radius: 10px;
    }
</style>