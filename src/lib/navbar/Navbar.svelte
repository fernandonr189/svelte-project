<script>
    import NavbarItem from "./NavbarItem.svelte";
    import NavbarItemLogo from "./NavbarItemLogo.svelte";
    import Fa from "svelte-fa";
    import { faD, faDoorOpen } from "@fortawesome/free-solid-svg-icons";
    import { faCircleChevronDown } from "@fortawesome/free-solid-svg-icons";
    import PrimaryButton from "../PrimaryButton.svelte";
</script>


<nav class="flex text-white bg-slate-900 p-3 justify-between items-center px-5">
    <NavbarItemLogo href="/" title="CyFer"/>
    <div class="md:inline-flex items-center hidden">
        <div class="px-2">
            <NavbarItem href="/" title="Home"/>
        </div>
        <div class="px-2">
            <NavbarItem href="/" title="About"/>   
        </div>
        <div class="px-2">
            <NavbarItem href="/" title="Products"/> 
        </div>
        <div class="px-2">
            <PrimaryButton func={
                console.log("Henlos")
            } title="Login" prefixIcon={faDoorOpen}/>
        </div>
    </div>
    <div class="md:hidden text-xl">
        <Fa icon={faCircleChevronDown} />
    </div>
</nav>