<script lang="ts">
    import { counter } from "./shared.svelte";

    function incrementCounter() {
        counter.count++;
    }
</script>
<button onclick={incrementCounter}>Click: {counter.count}</button>