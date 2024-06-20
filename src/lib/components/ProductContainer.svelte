<script>
    import PrimaryButton from "./PrimaryButton.svelte";
    import { faCreditCardAlt } from "@fortawesome/free-solid-svg-icons";
    import { faShoppingCart } from "@fortawesome/free-solid-svg-icons";

</script>


<div class="border-solid border-2 border-indigo-900 p-5 rounded-lg bg-slate-900">
    <div class="flex flex-col justify-center items-center">
        <img src="3060Ti.jpg" alt="cool-product" class="rounded-lg py-2">
        <p class="py-1 text-lg text-center">
            RTX 3060Ti Gigabyte
        </p>
        <p class="py-1 text-xl">
            $8900
        </p>
        <div class="p-2 flex flex-col items-center space-y-2">
            <PrimaryButton prefixIcon={faCreditCardAlt} title="Comprar"/>
            <PrimaryButton prefixIcon={faShoppingCart} title="Agregar al carrito"/>
        </div>
    </div>
</div>