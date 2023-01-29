<script lang="ts">
    //define props in typescript


    export let word:string = 'slovo';
    export let props:string;
    console.log(props)
    </script>
    
    {#if word===props}
    <li class="hidden">
        <span>{word}</span>
        <input type="text" class="border-2 py-1 m-2 text-center" bind:value={word}/> 
    </li>
    {/if}
    {#if word!==props}
    <li class="flex flex-col items-center   absolute">
        <span class="h-[40px] bg-white w-[90%]">{word}</span>
        <input type="text" class="border-2 py-1 m-2 text-center w-full" bind:value={word}/> 
    </li>
    {/if}