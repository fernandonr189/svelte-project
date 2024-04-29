<script>
  import NavBar from './lib/navbar/Navbar.svelte';
  import Home from './lib/routes/Home.svelte';
  import { Router, Link, Route } from 'svelte-routing'

  export let url
</script>

<main>
  <NavBar {url}/>
  <Router {url}>
    <Route path="/" component={Home}/>
  </Router>
</main>