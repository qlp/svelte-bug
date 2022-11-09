<script lang="ts">
    export let items: number[];
</script>
{#each items as i}
    <slot name="item" it={i}/>
{/each}
