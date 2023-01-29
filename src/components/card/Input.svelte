<script lang="ts">
export let word:string = 'slovo';
export let props:string = 'props';
</script>

{#if word===props}
<li class="hidden">
    <span>{word}</span>
    <input type="text" class="border-2 py-1 m-2 text-center" bind:value={word}/> 
</li>
{/if}
{#if word!==props}
<li class="flex flex-col">
    <span>{word}</span>
    <input type="text" class="border-2 py-1 m-2 text-center" bind:value={word}/> 
</li>
{/if}


