<script>
  import NavBar from './lib/navbar/Navbar.svelte';
  import Home from './lib/routes/Home.svelte';
  import Products from './lib/routes/Products.svelte'
  import About from './lib/routes/About.svelte';
  import Login from './lib/routes/Login.svelte';
  import Footer from './lib/footer/Footer.svelte';
  import Signup from './lib/routes/Signup.svelte';
  import { Router, Link, Route } from 'svelte-routing'

  export let url
</script>

<main>
  <NavBar {url}/>
  <Router {url}>
    <Route path="/" component={Home}/>
    <Route path="/products" component={Products}/>
    <Route path="/about" component={About}/>
    <Route path="/login" component={Login}/>
    <Route path="/signup" component={Signup}/>
  </Router>
  <Footer/>
</main>