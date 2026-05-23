<script lang="ts">
    let numbers = $state([1, 2, 3, 4, 5]);
    function totalNumber() {
        let total = 0;
        numbers.forEach((num) => {
            total += num;
        })

        return total;
    }

    function addNumber() {
        numbers.push(numbers.length + 1);
        console.log("Snapshot: " + $state.snapshot(numbers));
    }
    let total = $derived(totalNumber());
    //    let total = $derived(numbers.reduce((t, n) => t+n, 0));
    let copycat = $derived(numbers[numbers.length - 1]);
    $inspect("Inspect:" + numbers).with(helloWorld);
    function helloWorld() {
        console.log("Hello, World!");
    }
</script>

<div>{numbers.join('+')} = {total}</div>

<button onclick={addNumber}>Add</button>
<div>{copycat}</div>
