<script lang="ts">
    import TestSum from "./Component.svelte";
</script>

<TestSum
        items={[1, 2, 3]}
        let:it={i}>
    <span slot="item">{i}</span>
</TestSum>
<!-- this 'solves' the check error -->
{#if false}{#each [] as _}&nbsp;{/each}{/if}