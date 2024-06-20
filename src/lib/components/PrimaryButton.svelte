<script>
  import Fa from 'svelte-fa'
  export let prefixIcon = undefined
  export let sufixIcon = undefined
  export let func = () => {}
  export let title

</script>

<button on:click={func} class="bg-slate-900 shadow-sm hover:shadow-lg border-solid border-2 p-2 border-indigo-900 hover:bg-slate-950 rounded-lg h-fit">
  <div class="flex items-center">
    {#if prefixIcon !== undefined}
    <Fa icon={prefixIcon} class="mr-2 ml-1"/>
    {/if}
    <p>
      {title}
    </p>
    {#if sufixIcon !== undefined}
    <Fa icon={sufixIcon} class="mr-1 ml-2"/>
    {/if}
  </div>
</button>