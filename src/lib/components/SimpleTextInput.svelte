<script>
    export let type = "text"
    export let title = undefined
    export let placeholder = ""
</script>

<div class="py-2">
    {#if title !== undefined}
    <p class="py-2">{title}</p>
    {/if}
    <input {type} class="focus:bg-cyan-900 rounded-lg border-solid border-2 border-indigo-500 p-1 bg-cyan-950 outline-none shadow-lg w-full" {placeholder}>
</div>