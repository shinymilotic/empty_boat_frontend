<script>
	let elapsed = $state(0);
	let interval = $state(1000);

    $effect(() => {
        const id = setInterval(() => {
            elapsed += 1;
        }, interval);
        console.log("set Interval: " + id);
        return () => {
            clearInterval(id);
            console.log("Clear interval: " + id);
        };
    })
</script>

<button onclick={() => interval /= 2}>speed up</button>
<button onclick={() => interval *= 2}>slow down</button>

<p>elapsed: {elapsed}</p>
