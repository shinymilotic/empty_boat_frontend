<script lang="ts">
    let count = $state(0);

    function increment() {
        count += 1;
    }
</script>

<button onclick={increment}>Count: {count}</button>