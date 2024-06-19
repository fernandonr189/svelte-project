<script>
    import { faDoorOpen } from "@fortawesome/free-solid-svg-icons";
    import PrimaryButton from "../components/PrimaryButton.svelte";
    import SimpleTextInput from "../components/SimpleTextInput.svelte";
    import { Router, Link, Route } from 'svelte-routing'
</script>


<div class="bg-slate-800 flex text-white h-screen p-5 justify-center">
  <div class="md:flex bg-slate-900 rounded-lg p-10 h-fit w-fit shadow-lg">
    <div class="flex pl-5 pr-10 items-center">
      <img src="cool-keyboard.jpg" alt="cool-keyboard" class="rounded-lg">
    </div>
    <div class="flex flex-col justify-center items-center">
      <SimpleTextInput title="First name" placeholder="John"/>
      <SimpleTextInput title="Last name" placeholder="Doe"/>
      <SimpleTextInput title="Email" placeholder="example@site.com"/>
      <SimpleTextInput title="Password" type="password"/>
      <div class="pt-5 pb-2">
        <PrimaryButton prefixIcon={faDoorOpen} title={"Sign up"}/>
      </div>
      <div class="inline-flex text-xs">
        <p class="pr-2">Already a member?</p>
        <Link to="/login">log in</Link>
      </div>
    </div>
  </div>
</div>