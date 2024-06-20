<script>
    import PrimaryButton from "./PrimaryButton.svelte";



</script>


<div class="border-solid border-2 border-indigo-900 p-5 rounded-lg bg-slate-900">
    <div class="flex flex-col justify-center items-center">
        <img src="3060Ti.jpg" alt="cool-product" class="rounded-md py-2">
        <p class="py-1 text-lg text-center">
            RTX 3060Ti Gigabyte
        </p>
        <p class="py-1 text-lg">
            $8900
        </p>
        <div class="p-2 flex flex-col items-center space-y-2">
            <PrimaryButton title="Comprar"/>
            <PrimaryButton title="Agregar al carrito"/>
        </div>
    </div>
</div>