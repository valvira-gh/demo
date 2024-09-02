<script>
    import Reactive from "./Reactive.svelte";

    let creator = '<strong>vivapop</strong>';
    let appName = 'Svelte Demo App';
</script>


<header>
    <h1>Welcome to {appName}!</h1>
    <div>
        <p class="subtitle">My first sandbox demo with SvelteKit.</p>
        <p>Creator: {@html creator}</p>
    </div>
</header>

<div class="container">
    <Reactive />
</div>


<style>
    header {
        display: flex;
        flex-direction: column;
        align-items: center;
        border: 2px solid gray;

        && div {
            display: flex;
        }
    }

    .container {
        display: flex;
        border: 1px dotted black;
        justify-content: center;
    }
</style>