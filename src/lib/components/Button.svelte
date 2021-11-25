<script>
    import { createEventDispatcher } from 'svelte';
    export let label = 'button';

    const dispatch = createEventDispatcher();

    function doStuff() {
        dispatch('click')
    }

</script>

<button class='btn' on:click={ doStuff }>
    { label }
</button>