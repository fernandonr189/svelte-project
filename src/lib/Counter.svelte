<script>
  let count = 0
  const increment = () => {
    count += 1
  }
</script>

<button on:click={increment} class="bg-slate-900 shadow-sm hover:shadow-lg border-solid border-2 p-2 border-slate-400 hover:border-cyan-600 rounded-lg">
  Count is {count}
</button>
