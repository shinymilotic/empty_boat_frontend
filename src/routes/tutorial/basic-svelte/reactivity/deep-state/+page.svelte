<script lang="ts">
    let numbers = $state([1, 2, 3, 4]);

    function addNumber() {
        numbers.push(numbers.length + 1);
    }
</script>

<div>{numbers.join(', ')}</div>

<button onclick={addNumber}>
    Add Number
</button>