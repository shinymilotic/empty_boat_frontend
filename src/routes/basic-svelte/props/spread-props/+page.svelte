<script lang="ts">
    import Nested from "./Nested.svelte";

    const char = {name : 'Mai', address:"Binh Thai", genre:"Female"};
</script>

<Nested {...char} ></Nested>

