<script>
    import { faCartShopping } from "@fortawesome/free-solid-svg-icons";
    import PrimaryButton from "../components/PrimaryButton.svelte";
    import SimpleTextInput from "../components/SimpleTextInput.svelte";
    
    let counter = 0
    let increment = () => {
      counter += 1
    }
</script>


<div class="bg-slate-800 flex text-white h-screen p-5 justify-center">
    <div class="w-1/2">
        <SimpleTextInput placeholder="Busca en CyFer"/>
    </div>
</div>