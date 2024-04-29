<script>
    import { faCartShopping } from "@fortawesome/free-solid-svg-icons";
    import PrimaryButton from "../components/PrimaryButton.svelte";
    import SimpleTextInput from "../components/SimpleTextInput.svelte";
</script>


<div class="bg-slate-800 flex text-white h-screen p-5 justify-center">
  <div class="md:flex bg-slate-900 rounded-lg p-10 h-fit w-fit shadow-lg">
    <div class="p-5">
      <img src="cool-keyboard.jpg" alt="cool-keyboard" class="rounded-lg">
    </div>
    <div class="flex flex-col p-5 justify-center items-center">
      <SimpleTextInput title="Email" placeholder="example@site.com"/>
      <SimpleTextInput title="Contraseña" type="password"/>
    </div>
  </div>
</div>