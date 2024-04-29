<script>
    import { faCartShopping } from "@fortawesome/free-solid-svg-icons";
    import PrimaryButton from "../PrimaryButton.svelte";
    
    
    let counter = 0

  let increment = () => {
    counter += 1
  }
</script>


<div class="bg-slate-800 flex text-white h-screen p-5 justify-center items-center">
    <PrimaryButton prefixIcon={faCartShopping} func={increment} title="Count is {counter}: About"/>
</div>