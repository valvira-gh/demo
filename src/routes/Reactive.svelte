<script>
    let count = 0;

    function handleClick() {
        console.log('clicked')
        count += 1
    }
</script>

<button on:click={handleClick}>
    Clicked {count}
    {count === 1 ? 'time' : 'times'}
</button>

<style>
    button {
        font-size: 1.1rem;
        font-weight: 500;
        color: azure;
        border-radius: .5em;
        padding: .25em .5em;
        margin: 2em;
        background-color: rgb(10, 108, 255);
    }
</style>