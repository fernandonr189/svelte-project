<script>
  import Fa from 'svelte-fa'
  export let prefixIcon = undefined
  export let sufixIcon = undefined
  export let func
  export let title

</script>

<button on:click={func} class="bg-slate-900 shadow-sm hover:shadow-lg border-solid border-2 p-2 border-slate-400 hover:border-cyan-600 hover:bg-cyan-950 rounded-lg">
  <div class="flex items-center">
    <Fa icon={prefixIcon} class="mx-1"/>
    <p class="mx-1">
      {title}
    </p>
    <Fa icon={sufixIcon} class="mx-1"/>
  </div>
</button>