<script>
    import { Input } from "flowbite-svelte";
    import { ArrowDown } from "svelte-heros"
</script>

<div class="swap-main-div">
    <div class="swap-div">
        <Input type="number" value=0 size="lg"></Input>
        <div style="width: 100%; display: flex; justify-content: center;">
            <div style="cursor: pointer; background-color: rgba(0, 0, 0, 0.20); padding: 5px; border-radius: 10px;"><ArrowDown variation="outline"/></div>
        </div>
        <Input type="number" value=0 size="lg"></Input>
        <button class="trade-button" color="light">Trade</button>
    </div>
</div>

<style>
    .swap-main-div {
        margin-top: 20px;
        padding: 30px;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-wrap: wrap;
    }
    .swap-div {
        padding: 30px;
        background-color: white;
        max-width: 500px;
        border-radius: 15px;
        min-height: 300px;
        display: flex;
        justify-content: flex-start;
        flex-wrap: wrap;
        align-items: center;
        align-content: space-between;
    }
    .trade-button {
        width: 100%;
        background-color: black;
        color: white;
        padding: 15px;
        border-radius: 10px;
    }
</style>