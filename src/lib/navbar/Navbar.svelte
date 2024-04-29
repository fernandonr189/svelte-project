<script>
    import NavbarItem from "./NavbarItem.svelte";
    import NavbarItemLogo from "./NavbarItemLogo.svelte";
    import Fa from "svelte-fa";
    import { faCircleChevronDown, faDoorOpen } from "@fortawesome/free-solid-svg-icons";
    import PrimaryButton from "../PrimaryButton.svelte";
    import { Router, Link, Route } from 'svelte-routing'
    export let url
</script>


<Router {url}>
    <nav class="flex text-white bg-slate-900 p-3 justify-between items-center px-5">
        <NavbarItemLogo title="CyFer"/>
        <div class="md:inline-flex items-center hidden">
            <div class="px-2">
                <Link to="/">
                    <NavbarItem title="Home"/>
                </Link>
            </div>
            <div class="px-2">
                <Link to="/products">
                    <NavbarItem title="Products"/>
                </Link>
            </div>
            <div class="px-2">
                <Link to="/about">
                    <NavbarItem title="About"/>
                </Link>  
            </div>
            <div class="px-2">
                <Link to="/login">
                    <PrimaryButton title="Login" prefixIcon={faDoorOpen}/>
                </Link>
            </div>
        </div>
        <div class="md:hidden text-xl">
            <Fa icon={faCircleChevronDown} />
        </div>
    </nav>
</Router>