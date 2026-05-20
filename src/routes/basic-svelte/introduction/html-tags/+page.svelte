<script lang="ts">
    let title: string = "this string contains some <strong>HTML Tags</strong>";
</script>

<div>{title}</div>

<div>{@html title}</div>