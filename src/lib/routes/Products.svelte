<script>
    import { faCartShopping } from "@fortawesome/free-solid-svg-icons";
    import PrimaryButton from "../components/PrimaryButton.svelte";
    import SimpleTextInput from "../components/SimpleTextInput.svelte";
    import ProductContainer from "../components/ProductContainer.svelte"
    
    let counter = 0
    let increment = () => {
      counter += 1
    }
</script>


<div class="bg-slate-800 flex flex-col items-center text-white p-5 min-h-screen">
    <div class="w-1/2">
        <SimpleTextInput placeholder="Busca en CyFer"/>
    </div>
    <div class="grid lg:grid-cols-5 md:grid-cols-3 sm:grid-cols-2 gap-9 py-5 w-5/6">
        <ProductContainer/>
        <ProductContainer/>
        <ProductContainer/>
        <ProductContainer/>
        <ProductContainer/>
        <ProductContainer/>
        <ProductContainer/>
    </div>
</div>