<script>
  import PrimaryButton from './lib/PrimaryButton.svelte'
  import { faCartShopping } from '@fortawesome/free-solid-svg-icons'
  
  let counter = 0;

  let increment = () => {
    counter += 1
  }
</script>

<main>
  <div class="bg-slate-800 flex text-white h-screen p-5 justify-center items-center">
    <PrimaryButton func={increment} title="Count is {counter}"/>
  </div>
</main>