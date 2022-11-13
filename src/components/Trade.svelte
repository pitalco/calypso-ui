<script>
    import { Input, Button } from "flowbite-svelte";
</script>

<div class="swap-main-div">
    <div class="swap-div">
        <h2>Trade</h2>
        <Input type="number" value=0 size="lg"></Input>
        <Input type="number" value=0 size="lg"></Input>
        <Button size="xl" btnClass="swap-button">Trade</Button>
    </div>
</div>

<style>
    .swap-main-div {
        margin-top: 20px;
        padding: 25px;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-wrap: wrap;
    }
    .swap-div {
        padding: 25px;
        background-color: white;
        max-width: 500px;
        border-radius: 15px;
        min-height: 300px;
        display: flex;
        justify-content: center;
        flex-wrap: wrap;
        align-items: center;
        align-content: space-between;
    }
    .swap-input {
        min-height: 250px;
    }
    button {
        width: 100%;
    }
</style>